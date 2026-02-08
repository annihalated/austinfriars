---
title: "{{ replace .Name "-" " " | title }}"
date: {{ now.Format "2006-01-02" }}
layout: post
featured: false
url: /{{ .Name }}/
description: ""
draft: true
---
