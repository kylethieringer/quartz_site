---
title: how to run jupyter on hpc cluster
publish: "true"
timestamp: 2023-12-11 09:34
---
1. connect to tigressgateway

```bash
$ ssh kt1303@tigressgateway.princeton.edu
```

2. connect to spock

```bash
[kt1303@tigressgateway1 ~]$ ssh kt1303@spock.princeton.edu
```

3. change directory to folder with code

```bash
[kt1303@spock-login ~]$ cd /jukebox/murthy/Kyle/code
```

4. edit the `jupyter_spock.sh` file to specify the requested time and resources

```bash
[kt1303@spock-login code]$ nano jupyter_spock.sh
```

here is the `jupyter_spock.sh` file contents:
```bash
#!/bin/bash
#SBATCH --nodes=1
#SBATCH --ntasks=1
#SBATCH --cpus-per-task=1
#SBATCH --mem=4G
#SBATCH --time=02:00:00
#SBATCH --job-name=jupyter-notebook

# get tunneling info
XDG_RUNTIME_DIR=""
node=$(hostname -s)
user=$(whoami)
cluster="spock"
port=8889

# print tunneling instructions jupyter-log
echo -e "
Command to create ssh tunnel:
ssh -N -f -L ${port}:${node}:${port} ${user}@${cluster}.princeton.edu

Use a Browser on your local machine to go to:
localhost:${port}  (prefix w/ https:// if using password)
"

# load modules or conda environments here
module load anacondapy/2023.03
conda activate waggle

# Run Jupyter
jupyter-notebook --no-browser --port=${port} --ip=${node}
```

5. remove old slurm logs (just to make it easier to find current job)

```bash
[kt1303@spock-login code]$ ls
[kt1303@spock-login code]$ rm slurm-xxxxxx.out
```

6. submit the compute request

```
[kt1303@spock-login code]$ sbatch jupyter_spock.sh
```

7. open the log and copy the command to create the ssh tunnel on local machine

```bash
[kt1303@spock-login code]$ cat slurm-xxxxxx.out
```

on local machine copy and paste the line that looks like this:

```
ssh -N -f -L 8889:spock7-c2-4:8889 kt1303@spock.princeton.edu
```

will need to connect to vpn... (todo figure out way around this)
```bash
~ $ ssh -N -f -L 8889:spock7-c2-4:8889 kt1303@spock.princeton.edu
```

8. then scroll down to the server link that looks something like this:
```
http://127.0.0.1:8889/tree?token=3a55ebb93402a8979995e2806fb7bdb76aeab45
```

9. copy paste that into browser and begin working


10. kill the ssh tunnel on local machine

```bash
~ $ lsof -i 8889
```

this returns an id number for the tunnel

```bash
~ $ kill -9 xxxxx 
```

#🐛 | [[⨳ how to]]
## references
---
[princeton computing guide](https://researchcomputing.princeton.edu/support/knowledge-base/jupyter#sbatch)
