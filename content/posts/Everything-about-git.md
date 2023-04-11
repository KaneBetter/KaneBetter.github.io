---
title: "Everything About Git"
date: 2022-11-09T09:52:48-08:00
tags: [“Git”]
categories: ["Git"]
---

# The Perfect Commit

1. Add the <u>right</u> changes
   
   - Include changes for only one topic, `git add -p index.html`

2. Compose a <u>good</u> commit message, `git commit`
   
   - Subject = concise summary of what happened
   
   - Body = more detailed explanation
     
     - What is now different then before?
     
     - What's the reason for the change?
     
     - Is there anything to watch out for / anything particularly remarkable?

# Branching Strategies

### A Written Convention

Agree on a Branching Worflow in Your Team

- Git allows you to create branches but it doesn't tell you how to use them!

- You need a written best practice of how work is ideally structured in your team to avoid mistakes & collisions.

- It highly depends on your team / team size, on your project, and how you handle releases.

- It helps to onboard new team member ("this is how we work here").

### Integrating Changes & Structuring Releases

- Mainline Development (“Always Be Integrating”)
  
  - few branches
  
  - relatively small commits
  
  - high-quality testing & QA standards
- State, Release, and Feature Branches
  
  - different types of branches...
  - ..fulfill different types of jobs
  
- Long-Running & Short-Lived Branches
  - exist through the complete lifetime of the project
  - often, they mirror “stages" in your dev life cycle
  - common convention: no direct commits!

# Difference between git merge, git rebase, and git cherry-pick

- git merge will create commits in your branch. The commit will have all the changes in the branch that you want to merge. `git merge <branch>`

- `git cherry-pick <commit-ID> -n` no commit. git cherry-pick can only merge one commit after your changes.
- git rebase will rebase your changes into the branch you want to rebase. Your changes will be after the rebase branch changes.

`git config --global --list`

## Resource

- [Introduction to Git](https://www.notion.so/zarkom/Introduction-to-Git-ac396a0697704709a12b6a0e545db049)

- [Git for Professionals Tutorial - Tools &amp; Concepts for Mastering Version Control with Git - YouTube](https://www.youtube.com/watch?v=Uszj_k0DGsg)
