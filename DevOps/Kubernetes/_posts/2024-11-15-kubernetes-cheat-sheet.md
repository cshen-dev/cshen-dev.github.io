---
layout: post
title: "Kubernetes Cheat Sheet"
---



**Common Ad-hoc commands**

```
kubectl run -it sh *--image alpine*

kubectl run -it bash *--image ubuntu*

kubectl run -it build-deps *--image build-deps*

kubectl attach alpine -c alpine -i -t
```
