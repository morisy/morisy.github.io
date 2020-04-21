---
layout: post
title: Comparing Bit.ly, Google Analytics, and Drupal website logs
created: 1246553771
---
<span class="inline inline-right"><img src="http://morisy.com/files/images/bit_ly_downtime_0.jpg" alt="Bitly Fish" title="Bitly Fish"  class="image image-_original " width="268" height="195" /><span class="caption" style="width: 266px;"><strong>Bitly Fish</strong></span></span>Every Twitter user loves <a href="bit.ly" target="_blank">bit.ly</a>. It's simple. It's pretty. It's quick. It makes it easy to jump right into getting click through metrics and see who's actually reading your posts. But is it accurate? 

Particularly as compared to more "professional" tracking offerings out there, like Google Analytics or even a website's original logs, there have been concerns raised about how accurate those instantaneous numbers bit.ly gives out are. I've increasingly heard, for example, that bit.ly does a relatively poor job of parsing out bot traffic, which presumably just spiders through Twitter links looking for sites to spam.

I to test these services with an informal experiment: I would compare Bit.ly traffic against Google Analytics against my website's Drupal logs. I wasn't looking for the <em>perfect</em> solution, just to see how different the numbers these three reporting methods were giving.

The ground rules were simple: I would send out a <a href="http://twitter.com/morisy/status/2240789062">bit.ly'd link to Twitter</a>, explaining the test, and asking my followers to click if the wanted to. Polling would be closed at midnight, EST, but then I would look at the next few weeks to see if these alleged bots continued to inflate numbers.

The results were interesting, if not shocking, but some specific points about bit.ly, click tracking, and Twitter analytics should be noted:
<ul>
<li>It's a rapidly emerging field. If there is a problem with bots or something else inflating numbers, bit.ly will probably correct it as quickly as a public fuss is raised about it.</li>
<li>There's a lot of complicating factors that will leave Twitter click analytics a volatile field for a while. Already, I'm sure the rise of URL <em>elongating</em> services like <a href="http://longify.com/">Longify</a> have given these services a huge headache.</li>
<li>Even if Bit.ly isn't perfect, it's pretty damn good, and I think it's a reasonable question to ask if there is a "perfect" Twitter Analytics solution, or if there are just solutions better fit for your needs. Either way, I'm grateful they don't put obnoxious framing like Ow.ly does. And I don't mean to detract from Google Analytics, which is also a pretty powerful tool once you have it up and running.</li></ul>

But enough chit-chat, let's get to the meat: How did bit.ly stack up to Google Analytics and Drupal's own web logs? See for yourself:

<table width=300px align="center" border>
	<tr>
		<td>Service</td>
		<td># of recording hits on June 19, 2009</td>
	</tr>
	<tr>
		<td>Bit.ly</td>
		<td>12</td>
	</tr>
	<tr>
		<td>Drupal web logs</td>
		<td>26</td>
	</tr>
	<tr>
		<td>Google Analytics</td>
		<td>5</td>
	</tr>
</table>

So Bit.ly is more than two times higher than Google Analytics, but Drupal's logs (which I know for a fact are all too happy to count every last spam bot and betty) are twice that, and <b>five times</b> higher than Google Analytics.

A couple other things worth noting:
<ul><li>The Drupal test page was exclusively promoted through Twitter. It wasn't linked to from any other site, except through my Friend Feed which automatically aggregates my Tweets.</li>
<li>As a counter to the bot argument, after that first day of posting my Bit.ly link only registered one more click, and that was the next day, a completely reasonable time frame for a user to see the post.</li>
<li>Google Analytics registered 0 clicks after the first day of posting.</li>
<li>Drupal registered a handful (maybe 5) after the first few days.</li>
<li>In each of these three services, I made sure to remove any click I might have accounted for.</li></ul>

So, what do you think? Is Bit.ly still a useful tool? This is obviously a fairly small sample, but I'll keep an eye on how these tools stack up against each other over the next months, and hopefully have more data to share.

Besides, even at its worst, Bit.ly has got to have Conan O'Brien's "Twitter Tracker" beat:

<object width="512" height="296" align=center><param name="movie" value="http://www.hulu.com/embed/1zBuaeMsjlycG5flpHPNVA"></param><param name="allowFullScreen" value="true"></param><embed src="http://www.hulu.com/embed/1zBuaeMsjlycG5flpHPNVA" type="application/x-shockwave-flash" allowFullScreen="true"  width="512" height="296"></embed></object>

<b>Further Reading:</b>
<ul>
<li><a href="http://blog.bit.ly/">Bit.ly's excellent blog</a> which tackles a lot of these issues.</li>
<li><a href="http://www.hulu.com/watch/76852/the-tonight-show-with-conan-obrien-twitter-tracker#s-p9-st-i1">The original Twitter Tracker segment</a></li>
<li>A FriendFeed discussion of <a href="http://friendfeed.com/bhc3/619f00e6/something-is-very-wrong-with-bit-ly-click-counts">Bit.ly count problems</a></li>
<li>TechCrunch on <a href="http://www.techcrunch.com/2009/06/29/bitlys-grand-plans-and-their-inevitable-clash-with-digg-bitly-now/">Bit.ly's Grand Plans</a></li>
</ul>
