---
layout: post
name: git-usage-in-teams
title: Git usage in teams
date: 2017-06-14 13:00:00 +00:00
author: Cyryl Płotnicki
image:
   src: 
tags:
- git
- practices
- teamwork
- process
- workflow

---

Git workflows come in different shapes and forms. Typically though they fall into one of the two categories. The merge-based ones and the rebase-based ones. What I would like to do is to take you on a journey on which you decide which one suits your team best. 

Git popularity can be tracked down to it being used in some large open source projects. Imagine large codebases maintained by thousands of people over multiple years. The people communicate mostly via email and are spread out all over the world. They value ability to track down the reason for a change after months have passed. Imagine reading the code, asking git to annotate and being given a large commit clearly explaining the reasoning behind the change. All of the above made the communities to converge on rebase-based git workflows. 

[image]

You spawn a branch, you add commits there. You keep the multiple commits on the branch, as they help you do recording the steps you take. You issue a PR. When everyone is happy a **rebase on top of master** happens. Some time ago this would mean you do `rebase -i origin/master` and there, in the interactive mode, you say you want all of the commits squashed. Nowadays Github, Bitbucket and Gitlab all provide an option to do the squash from the UI, in some cases you still need to change the parent of the commit yourself though.

links:

* http://learngitbranching.js.org/

