---
title: "{{ replace .TranslationBaseName '-' ' ' | title }}"
date: {{ .Date }}
draft: false
category: ["membercard"]
first-name: ""
last-name: ""
affiliation: ""
address: ""
email: ""
orcid: ""
homepage: ""
profile-photo: "images/{{ .File.ContentBaseName }}.jpg"
---

