---
title: "Random Regex Snippets"
layout: post
date: 2022-02-06 10:44 −05:00
---

Just need a place to store these. Will hopefully add over time. 

First, some helpful resources:

* [Chua Hock-Chuan's guide to Regex's](https://www3.ntu.edu.sg/home/ehchua/programming/howto/Regexe.html)
* [Regex Extracter](https://github.com/zhangbohun?tab=repositories) by [Zhangbohun](https://blog.zhangbohun.com) for Chrome, which easily lets you run a regex right against a webpage your viewing.


### Extracting Datetime

Was trying to extract the datetime from some MuckRock html pages, and this was helpful interms of pulling just the date out of a given page:

```
datetime=.*\"
```

### Extracting Contacts from Sanebox

Very annoying, SaneBox doesn't let you export your trainings. Regex Extractor + a generic email extractor makes this less painful, though it's still a lot of clicking page after page:

```
(?:[a-z0-9!#$%&'*+/=?^_`{|}~-]+(?:\.[a-z0-9!#$%&'*+/=?^_`{|}~-]+)*|"(?:[\x01-\x08\x0b\x0c\x0e-\x1f\x21\x23-\x5b\x5d-\x7f]|\\[\x01-\x09\x0b\x0c\x0e-\x7f])*")@(?:(?:[a-z0-9](?:[a-z0-9-]*[a-z0-9])?\.)+[a-z0-9](?:[a-z0-9-]*[a-z0-9])?|\[(?:(?:(2(5[0-5]|[0-4][0-9])|1[0-9][0-9]|[1-9]?[0-9]))\.){3}(?:(2(5[0-5]|[0-4][0-9])|1[0-9][0-9]|[1-9]?[0-9])|[a-z0-9-]*[a-z0-9]:(?:[\x01-\x08\x0b\x0c\x0e-\x1f\x21-\x5a\x53-\x7f]|\\[\x01-\x09\x0b\x0c\x0e-\x7f])+)\])
```

Note that it also pulls in SaneBox's support contacts and your own email address around the page. This should have worked better because it pulls the email based on the HTML elements around it, but SaneBox pulls in this info via JavaScript and RegEx extractor wasn't playing nicely with that.

```
parts\.info\".*\>
```
