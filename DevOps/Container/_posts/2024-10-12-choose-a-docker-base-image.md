---
layout: post
title: "🐳 How to choose a  docker base image"
tags: [docker]
---


# How to choose a  docker base image

We are in favour of Debian based image due to pragmatic reason and its popularity in the open source community.

## Recent Debian release with code names

> Debian 12 (bookworm) — current stable releaseDebian 11 (bullseye) — current oldstable releaseDebian 10 (buster) — archived release, under third-party paid extended LTS supportDebian 9 (stretch) — archived release, under third-party paid extended LTS support

## Slim: Trimming the Fat for Efficiency

A “Slim” Docker image, often referred to as a “Slimmed-down” image, is an image that’s based on a certain distribution (like Debian) but has been optimized to be smaller by removing non-essential components. These images are created with the goal of reducing image size and improving efficiency while still maintaining necessary functionality for running applications.

## Debian vs Debian Slim

We prefer Debian Slim because of its optimized size.

## Debian Slim vs Alpine

We prefer Debian Slim for its compatibility and stability. However, we must acknowledge that Alpine excels in security and compilation speed.

