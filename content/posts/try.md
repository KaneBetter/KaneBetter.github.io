---
title: "Try"
date: 2022-04-10T12:00:51-07:00
draft: true
tags: [“bayes”]
categories: ["AA"]
---

# **Overview in Bazel**

Bazel is an open-source build and test tool similar to Make, Maven, and Gradle. It uses a human-readable, high-level build language. Bazel supports projects in multiple languages and builds outputs for multiple platforms. Bazel supports large codebases across multiple repositories, and large numbers of users.

# **LOC Statistics and Measuring**

At first, we used command `git ls-files | grep -E '.java' | xargs wc -l` to calculate the LOC of the cloned local repository. But rather than printing the numbers as a whole, it output the sums separately for several times.

Command Line Results

As an alternative we used other online tools like https://codetabs.com/count-loc/count-loc-online.html. As the whole project is too big for the site to compute (853 MB, mainly due to a large .git directory), we uploaded only the `/src` part of the project, and got the following result:

