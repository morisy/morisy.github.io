---
layout: post
title: What would you build on Twitter and Pushbutton?
created: 1249535684
---
<i><b>Author's Note:</b> This post is a work in progress. It is subject to revision, updates and possible deletion, so please, share your thoughts and help me better thing through it.-MM</i>
<p>
<p>After a night of <a href="http://www.hbo.com/entourage/" target="_blank">Entourage</a> and PBR, we got to talking about <a href="http://dashes.com/anil/2009/07/the-pushbutton-web-realtime-becomes-real.html">Anil Dash's Pushbutton Manifesto</a> (my term, his ideas) which would basically have a Twitter-like server in every home, or at least every home that wanted one, with a distributed, RSS-like real-time status update network.
<span class="inline inline-center"><img src="http://morisy.com/files/images/pushbutton.jpg" alt="" title=""  class="image image-_original " width="300" height="326" /></span>
<p>The essay and ideas fascinated me, and in something of a brainstorming session, I tried to come up with ways to make such a system useful. My first impulse, and the one that's stuck around all night, is a sort of <a href="http://morisy.com/tags/yahoo_pipes">Yahoo! Pipes</a> for the real-time Web.

<p>Both my friends are engineers, and both have Twitter accounts they almost never use. I spent the evening idly sketching out use cases. For example, parsing through: 
<ul><li>A user's current location (city or more specific), local Tweets, local event info and listings, friend's recent Tweets and locations</li></ul>
to get:
<ul><li>An event recommendation</li></ul>

<p>Then, I figured it would be relatively trivial to take take a <a href="http://howto.disqus.com/howto_rebooting_the_rss_cloud_88/">CloudRSS OPML</a>, for example, and parse that for popular URLs on a given subject or within a given community, kind of like an automagical niche Digg that is resistant to the dumbness of crowds.

<p>For example, rather than wading through all of the tweets from people Jay Rosen's following (as he suggest in one podcast) to get a pulse of what's going on in the Journalism Twitterverse, you take his Twitter OPML (which doesn't exist currently), use a Pushbutton server to grab all the recent updates, pull out the URLs people are Tweeting, and discover what articles are the most talked about in these categories.

<p>This creates a hand-curated social news feed that avoids the gaming and dumbing down that have hurt Digg as well as Reddit and Slashdot as the communities get more popular (I mean "hurt" quality and utility wise, as traffic has certainly gone up). Since it's a very controlled list of submitters (in this case, people who Jay Rosen thinks carry weight on journalism) I'm getting a very high signal-to-noise ratio. While a few people may post pictures of their cat, kids, or breakfast, few will retweet it so those posts won't make the news feed, and the signal will remain high (the number of RT's required to make the feed would be set in the Pipes-like application).

<p>With this Pushbutton pipes, I could then take, for example, the OPML list of people Jay Rosen is following, people the Boston Globe is following, and people the Boston Herald is following, and then parse out, for example, all the people more than 50 miles away. Then, if I wanted, only allow through Tweets with the word or tag "Boston," to get a local, Boston view from season journalists and sources.

<p>A couple more use cases:

<blockquote>
<h3>Bargain hunting</h3>
User drags a OPML list of Twitter accounts like <a href="http://twitter.com/bostontweet" target="_blank">@BostonTweet</a> or <a href="http://twitter.com/GroupOnBoston" target="_blank">GroupOnBoston</a>. Maybe the list is national.

<p>The user then narrows down the location they interested in, say, within 5 miles of Cambridge. Then, the user sorts for hash tags like #drink or #food from these users. Tweets with other hashtags might even get demoted for being "off topic," then Tweets without tags in the middle, then Tweets with the most tags on top. At the very top, the Pushbutton Pipes setup might sort the output by most times Re-Tweeted.
</blockquote>

<blockquote>
<h3>Apartment hunting</h3>
Apartment hunting is a relatively inefficient, horrible process, so this is just a first iteration but there's plenty of potential here. First, perhaps do a local search for #apartmentsforrent metadata, in Tweets, yes, but also Waves, another, more extensive real-time data storage.

<p>The user narrows it down to 4 choices that come up, some Tweets that lead to traditional Craigslist-style advertisements and other that are live, editable Waves. Since a certain amount of real-world relationships are shown, the renter sees he has several mutual connections with 2 of the landlords. He pings them, getting negative feedback on one landlord and positive on the other.

<p>One of the apartments the renter wasn't able to get a reference has a Wave, and so the renter asks some qualifying questions not addressed yet: Are pets allowed? What about parking? The answers are given out in the open, on the Wave, so the community can all see the updated apartment info. The Wave is associated with a showing time, which users can sign up for right on that page.

<p>The fourth apartment, with neither references nor a Wave to ask follow up questions, is left for later consideration if none of the earlier choices work out.
</blockquote>

Make sense? Think of other useful cases for a Pushbutton Pipes set up?

<p><p><b>Further Reading:</b>
<ul>
<li><a href="http://dashes.com/anil/2009/07/the-pushbutton-web-realtime-becomes-real.html">Anil Dash on Pushbutton ecosystem</a></li>
</ul>
