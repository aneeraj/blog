---
title: Kubernetes Debugging
date: 2023-08-16 01:00:00
tags:
- Quick Notes
categories:
- notes
keywords:
    - Kubernetes
    - k8s
---


#### Create an interactive shell on a Node:
    kubectl --context <cluster> debug node/<nodename> -it --image=mcr.microsoft.com/dotnet/runtime-deps:6.0

#### Delete debugging pod:
    kubectl delete pod node-debugger-mynode-pdx84 --now
