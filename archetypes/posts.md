---
title: "{{ replace .Name "-" " " | title }}"
date: {{ .Date }}
slug: {{ substr ( ( printf "%s%s" .Date .Name ) | base64Encode | sha256 ) -8 }}
description: ""
#cover: "cover.png"
tags: []
categories: []
---

Summary

<!--more-->