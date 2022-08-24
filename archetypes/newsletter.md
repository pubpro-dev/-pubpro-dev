---
title: "{{ replace .Name "-" " " | title }}"
summary: "{{ replace .Name "-" " " | title }}"
date: {{ .Date }}
author: "pubpro.dev"
ShowWordCount: false
draft: true
---

## New Cool Posts

{{ range first 10 ( where .Site.RegularPages "Type" "cool" ) }}
* {{ .Title }}
{{ end }}