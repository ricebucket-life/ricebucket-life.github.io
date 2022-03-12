---
title: Hello World
description: This site will mostly be used to document my homelab changes.
date: 2022-03-07
authors:
  - konri
draft: false
---

In order to understand how new technologies work, I need a hands-on practice environment to implement the latest technological changes. My homelab will be the pillar of my knowledge acquisitions. Maybe a career portfolio?

<!--more-->

## Homelab Philosophy

The idea for my homelab will be an hybrid on-premise and cloud environment. I will try to utilize free/affordable cloud services and incorporate it into my homelab.

### Existing Services

I already have some existing services that I need to note.

  - **Google Workspace for email services**

    I don't want to host email. Dealing with spam is a full time service and I rather not do that. Maybe in the future, I would host my own email server but for now, I am sticking to using Google Workspace. I had [Google G-Suite Legacy that was sunsetted on December 6, 2012 and will REALLY be sunsetted by May 1, 2022 with a forced upgrade to Google Workspace Starter Edition](https://support.google.com/a/answer/2855120?hl=en) ($5 per month per user). I already upgraded since Google provides [discounts](https://support.google.com/a/answer/60217) for early migrations to their paid business plan. I'll need to figure out if I want to continue to pay for this service or use something else, such as [Zoho](https://www.zoho.com/mail/zohomail-pricing.html) ($1/month/user) or [funnel everything into Cloudflare and have it forward to my personal gmail account](https://blog.cloudflare.com/introducing-email-routing/). 

  - **Cloudflare for DNS**

    I bought my domain using [porkbun.com](https://porkbun.com) registrar but decided to use Cloudflare's DNS service due to a lot of application support (Terraform, Ansible, etc). Cloudflare also provides email routing and web page caching, which I do not get with my domain registrar. I looked into [NS1](https://ns1.com) which has geographic filtering, which is pretty fancy for split horizen, but I'm going to stick with Cloudflare for now. I'll write a blog if I ever migrate to use NS1.

  - **Github for code respository**
  
    Github provides a free service to store my code publicly and privately. It was a hard choice between Github and GitLab but I'm sticking with Github due to popularity and maybe integration with Azure (if any) for future projects.


## Why Github Pages with Hugo

A fresh start on my homelab means I don't have any servers to host contents, as these servers are not yet configured. [Github Pages](https://pages.github.com) does not require me to run any servers or database backend and since I'm already using Github, it aligns with my homelab philosophy; *utilize free/affordable cloud services*. The website links are static pages so I don't need to care about security as much. It's also hosted on GitHub, thus, I don't need to worry about site performance or network bandwidth usage. 

I picked Hugo (over other static site generators, Jekyll, Pelican) due to popularity (more community support). Github allows me to Continuously Develop and Continuously Integrate via *Github Actions* to automatically generate static pages and push it publicly just by committing the changes to the repository. 

## What else am I using this site for?

- improve my technical writing
- journal my stock market ~~gambling~~ ideas.
- post photos that I took in which I think are good in my *PERSONAL* opinion. 
