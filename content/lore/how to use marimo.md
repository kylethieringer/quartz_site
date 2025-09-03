---
title: how to use marimo
publish: "true"
timestamp: 2025-08-28 12:28
---
marimo is a nice alternative to jupyter notebooks. the functionality is generally the same, but with a few distinct features that make it a bit nicer. marimo automatically runs dependent cells, so if you make a change early on, your variables stay up to date. it also prevents you from overwriting variable names in notebooks. this helps maintain reproducible code. and the workspace is all kept in a .py file so it can be run as a script. 

[see here for more details](https://docs.marimo.io/)

## remote marimo

access marimo using a remote server: 
```
ssh hostname # the remote computer

cd project/directory/

conda activate <environment>

marimo edit --headless --host 0.0.0.0 --port 8080
```

this will print out a url and attached is an access token. pay attention to this because you will need it to access the notebook.

then on local machine:
```
ssh -L 8080:0.0.0.0:8080 user@hostname
```

then go to 
`http://0.0.0.0:8080?<access token>