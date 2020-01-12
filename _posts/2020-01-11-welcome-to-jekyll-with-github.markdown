---
layout: post
title:  "Welcome to Jekyll and GitHub"
date:   2020-01-11 18:42:16 -0800
categories: netbob categories
---

This is the first experiment in programming websites with Jekyll and GitHub Pages

The procedure used for creating this website is as follows:

1. jekyll new ga_blog (or whatever) Create jekyll site
1.1 bundle exec jekyll serve (to create a localhost jekyll server to test content)
	- http://localhost:4000
	- ctrl-C to exit server
2. cd ga_blog
3. modify _config.yml (nano _config.yml)
	- add to baseurl "ga_blog" (for custom hosting replace this value with your full custom url here)
	- and save
4. Create repository on github with the name of your site folder. In this case its ga_blog
	- DON'T iniitialize the site on github. Just create it.
	- note the url in the github start new repository site: 
5. git init
6. git checkout -b gh-pages
7. git status (to list the files to be pushed up to gh-pages branch)
8. git add . (period means all files)
9. git commit -m "initial commit"
10. git remote add origin https://github.com/netbob/ga_blog.git (from the github repository create page)
11. git push origin gh-pages (note for me, it asked for my username and password. I am using 2fa so I had to create a new token (an app password aws it were for this to work)
12. Confirm on github gh-pages branch has the files you just pushed up.
13. go to the gh-pages branch and click on settings and scroll down to 
	- GitHub Pages
	- GitHub Pages is designed to host your personal, organization, or project pages from a GitHub repository.
	- Your site is published at https://netbob.github.io/ga_blog/
	- Confirm website is active on github under your username. Cool.
14. After making website changes:
	- git add . (or got add <specific pages>
	- git commit -m "optional comment"
	- git push origin gh-pages
