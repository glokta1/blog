---
title: "Cloud Native Buildpacks - MultiArch Support"
date: 2023-03-26T23:35:48+05:30
draft: false
cover:
    image: "https://buildpacks.io/images/buildpacks-logo.svg"
---

## Problem
 Currently `pack` can only build images for the same architecture as the host system. 

## Goal
 Provide option for cross compiling to different architectures and OS'es in `pack` CLI
 
## Understanding
- What are Cloud Native Buildpacks?
	- Dockerfiles vs CNBs https://tanzu.vmware.com/developer/blog/understanding-the-differences-between-dockerfile-and-cloud-native-buildpacks/
	- CNBs are readymade, rigorous, battle-tested `Dockerfiles` that you can include in your projects instead of making ones yourself. Saves time, improves security, at the cost of flexibility like with anything pre-made. Think pre-built PCs vs Custom PCs
- How is `pack` related to CNBs?
	- A CLI tool to use CNBs
- https://tanzu.vmware.com/developer/guides/cnb-what-is/
{{<figure src="https://cdn.hashnode.com/res/hashnode/image/upload/v1677566448430/94fffdec-0662-4e0e-8aa9-925facd7429e.jpeg" caption="Anatomy of a Builder" align="center">}}
## `pack` steps
1. Spin up container of builder img
2. Mount application source code on top of it
3. Invoke the `steps` binary present in the builder container which starts the Buildpack Lifecycle

### The Buildpack Lifecycle
{{<figure src="https://cdn.hashnode.com/res/hashnode/image/upload/v1677566485395/1e7d5888-1f25-4878-906b-35e104865baa.jpeg" caption="The writing's shit, I know." align="center">}}
https://miro.com/app/board/uXjVPrqGPB4=/
