---
layout: post
title:  "Project Mobile Application"
date:   2016-06-22
excerpt: "Minimal, one column Jekyll theme for your blog."
project: true
tag:
- suska cookies 
- app cache
- manifest
- about
- theme
comments: false
---

## Application Cache On HTML5

HTML5 saat ini memberikan keleluasaan bagi developer untuk dapat data situsnya pada client, jadi ketika client offline sekalipun , situs masih bisa dibuka.

> Installation

```
<!DOCTYPE>
<html manifest="site.manifest">
<head>
	<title>Cache</title>
</head>
<body>
	<h1>Application Cache</h1>
</body>
</html>
```
> Save into index.html
* Value parameter is the file extension manifest manifest that lists the files that we store on the client to be accessible even when you're offline .

```
CACHE MANIFEST
# version 0.1

index.html
```
> Save into site.manifest

```
AddType text/cache-manifest manifest
 ```
> Save into .htaccess

We Are [Uin Suska Riau] from [Information System].

[Uin Suska Riau]: http://uin-suska.ac.id
[Information System]: http://sif.uin-suska.ac.id/
