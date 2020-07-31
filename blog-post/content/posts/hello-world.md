---
title: "Whats The Deal With Static Websites?"
date: 2020-07-30T21:50:56-04:00
draft: false
---

I feel like it was not long ago that I was using Adobe Dreamweaver to work on my website for my Bachelor Degree final project. It was some lame website that had to be a functioning computer ecommere website, think Dell's website where you can customize computers. I wrote it in Java with JSTL on the front end to handle server side rendering.

Now in 2020 its becoming a super hot topic to make static websites, as if it was never a bad thing? I'm sitting here typing this blog post inside of a markdown file, no HTML syntax involved at all. It's so bizzare, a website without HTML.

You might be asking, well how am I doing? I'm using this new framework written in Go called Hugo. Its a static site generator, where you plug-in some config, choose a template, and I'm done. No CSS to worry about, no complicated dynamic content. Its just easy. When I want to write a new post, I can just push the file to my repo, and then have a Github Workflow setup or DevOps CI/CD pipeline to compile the site and publish it whereever.

In my case this website is running on Azure Storage with Statis Web App enabled. I pieced together two GitHub workflows, one that builds the hugo site and another that uploads to the storage account.