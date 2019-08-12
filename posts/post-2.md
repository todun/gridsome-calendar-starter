---
title: Post 2
excerpt: GitLab pages allows you to deploy static websites using their CI tools.
date: 2019-08-12T07:30:42.696Z
---
GitLab pages allows you to deploy static websites using their CI tools.



First, you need to make a few preparations:



Set correct base in gridsome.config.js:

If you are deploying to https://<USERNAME or GROUP>.gitlab.io/, you can omit pathPrefix as it defaults to "/".



If you are deploying to https://<USERNAME or GROUP>.gitlab.io/<REPO>/, (i.e. your repository is at https://gitlab.com/<USERNAME>/<REPO>), set pathPrefix to "/<REPO>/"



Set outDir in gridsome.config.js to 'public'.

Create a .gitlab-ci.yml file in the root of your project with the content below. This will build and deploy your site whenever you make changes to your content.
