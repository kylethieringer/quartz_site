---
title: connecting a github pages site to a custom domain
tags:
  - 🦋
publish: "true"
---
this process involves directing a github pages site to a custom domain and a custom subdomain.

the default github-pages domain name is `<your-github-repo>.github.io` and this is totally fine when getting things started. this just walks through the steps I needed to take to use my own custom domain.
## hosting a github pages on a custom domain
I am hosting my personal website in one github repo that uses the [al-folio jekyll theme](https://github.com/alshedivat/al-folio) and deploys to a custom **domain** name: www.kylethieringer.com. setting this up is fairly straightforward:
1. fork or clone the repository for the theme to your own github account.
2. edit the site and deploy locally to test how it will look
3. add the custom domain to the github pages section in the repo's settings (like `kylethieringer.com`.
	- this will probably throw out a bunch of errors like "DNS settings not configured correctly" or "cannot verify security settings". Don't worry these will go away on their own with time!
4. navigate to your website hosting settings and go to the custom DNS settings.
5. add custom DNS settings as per the [github recommendations](https://docs.github.com/en/pages/configuring-a-custom-domain-for-your-github-pages-site/managing-a-custom-domain-for-your-github-pages-site) 
	- you will need to create 4 DNS `A` records with slightly different IP addresses
	- you will need to create a `CNAME` record that points to your github account: `kylethieringer.github.io` (NOTE: it does not specifically point to your repo)

	- heres what my DNS settings look like:
	- ![[DNS_settings.png]]

6. give this time reconfigure. it takes anywhere from a couple hours to a couple of days for the global DNS settings to adjust where they point to and fully update. Dont panic if you get messages about security issues or misconfigured settings. just be patient.
7. the repository readme has instructions about deploying the website. Heres the quick overview of how Im doing it for the main website:
	- I am deploying from a branch in the settings (the `gh-pages` branch of the repo)
	- the repo has some deployment settings built in so that every time I commit changes to the repo it automatically starts the deployment steps and just takes a few moments to become live
	- For example, my workflow using the [al-folio template site](https://github.com/alshedivat/al-folio) is just simply this:
	```bash
	~ ❯ cd Documents/website
	~/Documents/website master ❯ git status
	~/Documents/website master ❯ git add .
	~/Documents/website master ❯ git commit -m "commit message"
	~/Documents/website master ❯ git push
	```

	- to deploy a local version of the website for testing, there are some slightly different steps:
	1. First, I created a [virtual conda environment](https://conda.io/projects/conda/en/latest/user-guide/getting-started.html)
	2. I installed jupyter into that environment
	3. I needed to install a different version of ruby onto my computer, than what was already installed by default. To do this, I installed [chruby](https://formulae.brew.sh/formula/chruby) with [homebrew](https://brew.sh/). I can then run the command `chruby ruby-3.2.2` before the next steps to make sure everything runs ok
	4. in the conda environment, and in the website project folder, I start a local server with this command: `bundle exec jekyll serve --lsi`

## hosting a github pages site on a custom subdomain
my notes are hosted on a custom **subdomain** through a separate github repository. The custom domain is set to `notes.kylethieringer.com`

the steps to follow are very similar as using the custom domain. All you need to do is add an additional `CNAME` record to the website hosting DNS settings that replaces the `www` with the custom subdomain (in my case `notes`). Then in the pages settings, make sure deploy from action is selected, instead of deploy from branch like the previous section.

Quartz has a bit fancier way to deploy the site because it has to do some local processing before syncing with the github repo. [the online guide](https://quartz.jzhao.xyz/authoring-content#syncing-your-content)explains all the steps to take when adding and syncing notes to the hosted site. 

heres a quick overview of how I update my notes website with new notes from obsidian:
```bash
~ ❯ cd /Users/kyle/Library/Mobile\ Documents/iCloud~md~obsidian/Documents/notes_publish
~ ❯ npx quartz sync
~ ❯ npx quartz build
```

executing `npx quartz build --serve` runs a local server for testing the website as well.


#🦋 | [[how I made this site]] | [[⨳ how to]]