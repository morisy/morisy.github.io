---
layout: post
title: 'Drupal: Facebook Connect or not to connect ...'
created: 1257369077
excerpt: !ruby/string:Sequel::SQL::Blob "<i><b>Editor's Note:</b> In the interest
  of sanity and others' edification, I thought it might be nice to start logging my
  travails developing <a href=\"http://sparechangenews.net/\">Spare Change News</a>
  in Drupal. I probably won't post all the updates to Instant History (the main blog),
  but the major ones will show up there, with everything cross-posted to the new <a
  href=\"http://morisy.com/tags/drupal_developer_blog\">Drupal Developer blog</a>
  (It's all really just one blog with different categories, but shh ...).</i>\r\n\r\nSo
  far, one of the biggest challenges I've run into with <a href=\"http://sparechangenews.net/\">Spare
  Change</a> is getting staff to actually log in and post content. The most common
  excuse? \"I can't remember my user name and password.\" It's a sentiment I'm sympathetic
  to, having written about <a href=\"http://itknowledgeexchange.techtarget.com/IT-watch-blog/everyone-hates-your-insecure-password-rules/\">user
  hatred of password rules</a>. But what's a site admin to do? \r\n\r\n<a href=\"http://morisy.com/facebook_connect_or_not_connec#continuedt\">Continued&gt;&gt;</a>\r\n"
---

<i><b>Editor's Note:</b> In the interest of sanity and others' edification, I thought it might be nice to start logging my travails developing <a href="http://sparechangenews.net/">Spare Change News</a> in Drupal. I probably won't post all the updates to Instant History (the main blog), but the major ones will show up there, with everything cross-posted to the new <a href="http://morisy.com/tags/drupal_developer_blog">Drupal Developer blog</a> (It's all really just one blog with different categories, but shh ...).</i>

So far, one of the biggest challenges I've run into with <a href="http://sparechangenews.net/">Spare Change</a> is getting staff to actually log in and post content. The most common excuse? "I can't remember my user name and password." It's a sentiment I'm sympathetic to, having written about <a href="http://itknowledgeexchange.techtarget.com/IT-watch-blog/everyone-hates-your-insecure-password-rules/">user hatred of password rules</a>. But what's a site admin to do? 

<a name="continued"></a>Well, Drupal just so happens to have an excellent <a href="http://drupal.org/project/fbconnect">Facebook Connect module</a>, that just so happens to work great. I managed to get it working within just a few minutes on this very site (you can check it out here: <a href="http://www.morisy.com/user">http://www.morisy.com/user</a>).

I really like the module for a number of reasons:
<ul><li>Unlike <a href="http://disqus.com/">Disqus</a>, the commenting service I've long been wary of, the Drupal Facebook connect module creates a *local* user, and I control how that user is administered, I keep a local copy of their comments, and <b>my</b> site controls how that data is used, not a third party</li>
<li>It's simpler than OpenAuth, OpenID and other federated login systems. I love the idea, but implementations are just plain confusing. On a site dedicated to homeless issues, we have to assume a low level of tech savvy (this complexity might change soon with <a href="http://googleblog.blogspot.com/2009/11/cutting-back-on-your-long-list-of.html">Google making a big push on usability</a>).</li>
<li>It works. I would say "It just works," but a Drupal forums user pointed me to the <a href="http://drupal.org/project/issues/fbconnect?categories=All">bug queue</a>. Are there issues? Absolutely, but I'm willing to quash them as they come up for the sake of usability.</a>
</ul>

Now, when I eventually want to upgrade to a more generic module that accepts Facebook, Google, and whatever else you can throw at it ... That's when I expect some issues. But that will be another day.
