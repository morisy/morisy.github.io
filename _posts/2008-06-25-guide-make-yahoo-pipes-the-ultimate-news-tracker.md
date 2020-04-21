---
layout: post
title: 'Guide: Make Yahoo! Pipes the ultimate news tracker'
created: 1214373039
---
<p>A few summers ago, I was guest editing a blog that covered a few topics I had only loosely tracked before. Since my job was to find and post the most interesting overlooked bits, I gave <a href=http://pipes.yahoo.com/pipes/>Yahoo! Pipes</a> a look as a way to create a “news scanner,” and I was really happy with the <a href=http://pipes.yahoo.com/pipes/pipe.info?_id=74e440d49fdb7c0fef2c41881ab82b62>result, dubbed IvyTrack</a> ... when it worked.

<p>Unfortunately, RSS feeds had a knack for not loading, but today I’m giving it another go with a guide on how to set up your own news topic tracker, including ways to get instant alerts through AOL IM or GChat when news on your beat breaks. Today, it’s all about speed, and Yahoo! Pipes can be a great tool on getting the heads up.

<a href=http://www.morisy.com/yahoo-pipes-guide-to-tracking-news>Read on for the full guide ...</a>
<!--break-->
<p>
<p><b>1. Log in to Yahoo! Pipes</b>

<span class="inline right"><a href="/" onclick="launch_popup(62, 640, 532); return false;" target="_blank"><img src="http://www.morisy.com/files/images/Picture%201.thumbnail.png" alt="" title="" class="image thumbnail" height="83" width="100"></a></span>


<p>Just head over to <a href=http://pipes.yahoo.com/pipes/>http://pipes.yahoo.com/pipes/</a> and log in with your Yahoo! account. Don’t have one yet? For shame! Though they try to hide it, Yahoo! has some really great, innovative technology, and Pipes is one of my favorites.

<p><b>2. Build off a template</b>

<p>No sense reinventing the wheel. I’ve used a pared down <a href=http://pipes.yahoo.com/pipes/pipe.info?_id=74e440d49fdb7c0fef2c41881ab82b62>IvyTrack v2</a> as my template, and you can, too, since Yahoo! Pipes lets you copy and edit any public, existing pipes. Simple click the link and click “Clone.”

<p>After a brief loading sequence, you should see a list of (more or less) Ivy League related stories: 



<span class="inline left"><a href="/" onclick="launch_popup(63, 640, 543); return false;" target="_blank"><img src="http://www.morisy.com/files/images/pic2.preview.png" alt="IvyTrack Template" title="IvyTrack Template" class="image preview" height="543" width="640"></a><span class="caption" style="width: 638px;"></span></span>




<p>Great! Now, click the title and let’s rename it something more appropriate. Since I’m tracking networking equipment vendors these days, I’ll call mine <a href=http://pipes.yahoo.com/pipes/pipe.info?_id=9f278521021e294e2dac973d472161f9>CiscoTrack v1</a>, and change the description below the title as well. Now it’s time to dig into the guts of Pipes.

<p><b>3. Edit the template to include Google news search</b>

<p>Click edit source, and your browser should go to a page that looks pretty close to the one on the right. We see a bunch of URLs, a bunch of blue connectors, and some other techno mumble jumble. Lets start on the far left, with the bubble menu entitled “Feed Auto-Discovery.” This menu lets you put in a number of website URLs and figures out where their RSS feeds are. It’s simpler than finding the data which Pipes usually works with, which is the RSS feed itself. This particular bubble box has all the <a href=http://news.google.com/>Google News</a> alerts I’m interested in tracking, which I found more convenient then signing up for dozens of daily e-mail alerts.


<span class="inline left"><a href="/" onclick="launch_popup(64, 640, 356); return false;" target="_blank"><img src="http://www.morisy.com/files/images/Picture%203.preview.png" alt="CiscoTrack" title="CiscoTrack" class="image preview" height="356" width="640"></a><span class="caption" style="width: 638px;"></span></span>


<p>I’m not interested in tracking these topics for my networking equipment feed, and you probably aren’t either, so let’s go ahead and delete all those particular alerts. Simply click the minus sign by each URL. Afterwards, in the Feed Auto-Discovery bubble, you should just have a plus sign next to the words “Page URL”.

<p>Now lets go back to <a href=http://news.google.com/>Google News</a> and do a search for a topic we’re interested in. “Cisco” is a good place to start, and the results are pretty on target with what I’m interested in. Just copy the URL that comes up (in this case <code>http://news.google.com/news?hl=en&ned=&q=cisco&btnG=Search+News</code>), go back to Pipes, hit the plus sign in Feed Auto-Discovery, and insert the link. After a few seconds, Pipes should figure out where the RSS feed is and start piping in your fresh new search.

<p>To check and see that the items are going through, click the “Loop” bubble below “Feed Auto-Discovery.”




<span class="center"><a href="/" onclick="launch_popup(65, 566, 380); return false;" target="_blank"><img src="http://www.morisy.com/files/images/Picture%205.png" alt="" title="" class="image preview" height="380" width="566"></a></span>





<p>You can then instantly see all the results Google News will return. The reason you have to run “Feed Auto-Discovery” through a loop that looks like it does nothing is because by itself “Feed Auto-Discovery” just returns the URL of the RSS feeds it discovers. After running through the “Loop” function and having Loop “Fetch Feed” URLs, Pipes will return the actual content you’re interested in.

<p>Another company I track is <a href=http://www.arubanetworks.com/>Aruba Networks</a>, but do a search for “Aruba” and way way too much noise comes back. We’ll modify the Google News search to be <code>"aruba networks" OR (aruba ARUN)</code> which will have a smaller scope but will still get most of what we’re interested in, and then copy the URL as before into a new slot.

<p><b>4. Include other news sources</b>

<p>This continues on with all the Google news topics you are interested in. In the second column, I used a similar search method except with a <a href=http://technorati.com/search/cisco+OR+%22aruba+networks%22+OR+juniper?authority=a4&language=en>Technorati blog search</a>.  Feel free to experiment with your own favorite search engine, like <a href=http://summize.com/search?q=cisco>Summize</a> to track Twitter conversations if that interests you.

<p>Finally, in my third and final column I include websites where all the content is relevant. The three different columns are just used to keep the organization neat, but you can have as many or as few as you want.

<p>In this third column, I’ll typically include related blogs, news sites, press home pages, and other pages dedicated to the topic I know will have what interests me. If you know a site doesn’t have an RSS feed, or if Pipes is having trouble figuring out how to parse it, you can try out <a href=http://feedity.com/>Feedity</a> which takes any site and creates an RSS page out of its changes, quite a useful trick for those content creators behind the curve.


<p><b>5. What happens to your feeds</b>

<p>Now that all those discovered feeds are fed into their respective loops, they are then piped through the “Union” widget, which pools all the outputs together. After that, it’s through the “Unique” widget which makes sure that if the same story is pulled from two sources (say, Aruba and Cisco are both mentioned in one story picked up by Google News) you only get the link once.

<p>Once all that is done, it’s piped to “Pipe Output,” which is where we get our final product, which we can now proudly view by clicking save and “Run Pipe.”

<p><b>6. Getting real-time updates by IM or txt message</b>
<p>There's a lot of services out there that claim to convert RSS to IMs, but the only one I found working when I wrote this was <a href=http://inezha.com/>Inezha</a>. I have no idea what the name means, but it's fairly simple to sign up and have it convert your Yahoo! Pipes output page to chats. You can set the interval for updates by typing "Timer" and then the time, in minutes, between updates you want.

<p>For those who are really brave, Yahoo! has an option to add a mobile device and get text message alerts: Just click “Results by Email or Phone.” 

<p>Phew. And we’re finally done! You can see <a href=http://pipes.yahoo.com/pipes/pipe.info?_id=9f278521021e294e2dac973d472161f9>my final product</a>, and feel free to leave any questions or tips of your own in the comments, or check out further reading for some other ideas and advanced Pipes techniques.
 
<p><b>Further Reading:</b>
<ul>
<li><a href=http://www.jumpcut.com/fullscreen?id=F4396574585311DC87A2000423CF0184&type=clip>Yahoo!’s video walkthrough and introduction to Pipes</a></li>
<li><a href=http://blogs.open.ac.uk/Maths/ajh59/014351.html>One experiment to try and turn a Pipe into a live audio feed</a>, something I’d like to try to do to create a police scanner feel.</li>
<li><a href=http://onlinejournalismblog.com/2008/04/25/something-for-the-weekend-6-mashups-with-yahoo-pipes/>A few journalism-related Yahoo! Pipes resources</a></li>
</ul

<i><b>Note:</b> For whatever reason, the vast majority of comment spam this blog received was on this page. Comments have been disabled as of June 15, 2009, but feel free to contact me as described in the sidebar.</i>
