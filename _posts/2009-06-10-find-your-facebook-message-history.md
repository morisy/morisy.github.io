---
layout: post
title: Find your Facebook message history
created: 1244613051
excerpt: !ruby/string:Sequel::SQL::Blob "After my posts on how to <a href=\"http://morisy.com/facebook_virus_attacks_continues_check_kirgoat_nutpicat_and_brungaat_continue_lure_unwary\">fix
  the Facebook virus</a> after an attack, I've noticed a number of searchers looking
  for information on how to find a particular message in your Facebook message history.
  I've put together a <a href=\"http://morisy.com/find_your_facebook_message_history\">Facebook
  message search guide</a> to help just these people, including some bad news about
  Facebook chat history. <small><a href=\"http://morisy.com/find_your_facebook_message_history\">Read
  the full post.</a></small>\r\n"
---

After my posts on how to <a href="http://morisy.com/facebook_virus_attacks_continues_check_kirgoat_nutpicat_and_brungaat_continue_lure_unwary">fix the Facebook virus</a> after an attack, I've noticed a number of searchers looking for information on how to find a particular message in your Facebook message history.

<blockquote><b><i>Update:</b> I've created a seperate guide to <a href="http://morisy.com/how_log_and_pull_your_facebook_chat_history">record and read Facebook chats</a>. This covers non-chat messages.</blockquote>

Fortunately, things have improved a lot since Facebook messaging was declared "completely unusable as a personal or business productivity tool" by <a href="http://www.techcrunch.com/2008/05/03/urgent-changes-are-needed-to-facebook-messaging/">Michael Arrington of TechCrunch</a> over a year ago.

Facebook apparently heard Arrington's complaint and finished up the <a href="http://blog.facebook.com/blog.php?post=20387467130">Facebook message search</a> they'd been working on.

<h3>Finding Facebook messages with Facebook message search</h3>
<span class="inline inline-right"><img src="http://morisy.com/files/images/n20531316728_1037065_4654.jpg" alt="facebookMessage" title="facebookMessage"  class="image image-_original " width="242" height="70" /><span class="caption" style="width: 240px;"></span></span>I'd highly recommend starting with Facebook's own message search. Unlike Google, not all of Facebook's searches are neatly integrated into their default search, but click on "Inbox" and then, right below "Compose Message," you have "Search Inbox."

It's grayed out, so dock points for usability, but at least it's there, right? One important note: The search index for Facebook messages seems to update relatively slowly, so recent messages will <b>not</b> likely appear in your search results, even if they include the words you're searching for. It's also important to note that, if you begin typing in a contact's name, Facebook will autocomplete for you and pull up all the messages from that individual.

<h3>Finding Facebook messages with GMail</h3>

My personal preference is to use GMail, which works great if you use GMail, but is totally useless if you don't/didn't use it for your Facebook account. The benefit is that you can use GMail's powerful search functionality to find exactly the message thread you are interested in. Finding just one message from that thread will provide you with the link to the original message ... and its entire conversation, so if you can find a piece of what you're interested in, Facebook will guide you the rest of the way.

To make things a bit quicker, if you regularly refer to Facebook messages or find yourself struggling with the search parameters, I've created a couple of bookmarks, courtesy of the <a href="http://eclectic-mayhem.com/stuff/gmail-search-bookmarks.html">GMail Search Bookmarks</a> homepage, that you can simply drag up to your browser (or right-click on and save manually). Clicking on them later will bring up the query you're looking for:
<br>
<p align="center"><table align="center" border="1" bordercolor="#000000" style="background-color:#FFFFFF" width="500" cellpadding="3" cellspacing="3" >
	<tr>
		<td>Bookmarklet <br><small>(Drag to linkbar!)</small></td>
		<td>What it does</td>
	</tr>
	<tr>
		<td><a href="javascript:%28function%28%29%7Bvar%20base%3D%22http%3A//mail.google.com/mail/%22%3Bif%28location.href.indexOf%28base%29%3D%3D0%29%7Bvar%20f%3Dwindow.frames%5B0%5D.frames%5B0%5D.document.getElementById%28%22s%22%29%3Bvar%20inputs%3Df.getElementsByTagName%28%22input%22%29%3Bvar%20q%3Dnull%3Bfor%28var%20i%3D0%3Bi%3Cinputs.length%3Bi++%29%7Bif%28inputs%5Bi%5D.name%3D%3D%22q%22%29%7Bq%3Dinputs%5Bi%5D%3B%7D%7Dq.value%3D%22from%3Afacebookmail.com%20%22sent%20you%20a%20message%22%22%3Bf.onsubmit%28%29%3B%7Delse%7Blocation.href%3Dbase+%22%3Fsearch%3Dquery%26q%3Dfrom%253Afacebookmail.com%2520%2522sent%2520you%2520a%2520message%2522%26view%3Dtl%26fs%3D1%22%3B%7D%7D%29%28%29">Facebook Messages</a></td>
		<td>Shows all your Facebook messages</td>
	</tr>
	<tr>
		<td><a href="javascript:%28function%28%29%7Bvar%20base%3D%22http%3A//mail.google.com/mail/%22%3Bif%28location.href.indexOf%28base%29%3D%3D0%29%7Bvar%20f%3Dwindow.frames%5B0%5D.frames%5B0%5D.document.getElementById%28%22s%22%29%3Bvar%20inputs%3Df.getElementsByTagName%28%22input%22%29%3Bvar%20q%3Dnull%3Bfor%28var%20i%3D0%3Bi%3Cinputs.length%3Bi++%29%7Bif%28inputs%5Bi%5D.name%3D%3D%22q%22%29%7Bq%3Dinputs%5Bi%5D%3B%7D%7Dq.value%3D%22from%3Afacebookmail.com%22%3Bf.onsubmit%28%29%3B%7Delse%7Blocation.href%3Dbase+%22%3Fsearch%3Dquery%26q%3Dfrom%253Afacebookmail.com%26view%3Dtl%26fs%3D1%22%3B%7D%7D%29%28%29">Facebook Notifications</a></td>
		<td>Displays all your Facebook notifications, including messages</td>
	</tr>
	<tr>
		<td><a href="javascript:%28function%28%29%7Bvar%20base%3D%22https%3A//mail.google.com/mail/%22%3Bif%28location.href.indexOf%28base%29%3D%3D0%29%7Bvar%20f%3Dwindow.frames%5B0%5D.frames%5B0%5D.document.getElementById%28%22s%22%29%3Bvar%20inputs%3Df.getElementsByTagName%28%22input%22%29%3Bvar%20q%3Dnull%3Bfor%28var%20i%3D0%3Bi%3Cinputs.length%3Bi++%29%7Bif%28inputs%5Bi%5D.name%3D%3D%22q%22%29%7Bq%3Dinputs%5Bi%5D%3B%7D%7Dq.value%3D%22from%3Afacebookmail.com%20%22sent%20you%20a%20message%22%22%3Bf.onsubmit%28%29%3B%7Delse%7Blocation.href%3Dbase+%22%3Fsearch%3Dquery%26q%3Dfrom%253Afacebookmail.com%2520%2522sent%2520you%2520a%2520message%2522%26view%3Dtl%26fs%3D1%22%3B%7D%7D%29%28%29">Secure Facebook on GMail</a></td>
		<td>Facebook through GMail via HTTPS</td>
	</tr>
</table>
<br>
If using those buttons alone doesn't do the trick, the search query is saved in your "Search" bar in GMail, and you can add terms ranging from people's names ("Lisa," "Michael") to key words ("picnic," "social networking"). 

<h3>Searching Facebook instant message history</h3>

Now for the bad news: If you're looking to search through old Facebook <b>chats</b>, as opposed to <b>messages</b>, you're out of luck. According to message on Facebook's <a href="http://www.facebook.com/help.php?page=824">official FAQ</a>, the site does not permanently keep chat history ...fow now:
<blockquote>You can view recent conversation history by opening a chat window with your friend. You cannot view older conversations at this time or conversations with friends who are not currently online.

To clear your chat history just click the "Clear Chat History" link at the top of your Chat window. While message history is saved from page to page, and even between login sessions, please note that it is not logged permanently.</blockquote>

To delete even that temporary cache of conversation, simply open up a conversation with the person on the other end of the chat and click "Clear History."

<b>Further Reading:</b>
<ul>
<li>What to do if you get hit by the <a href="http://morisy.com/what_do_if_you_get_hit_facebook_brungaat_virus_attack">Facebook brunga.at virus attack</a></li>
<li><a href="http://morisy.com/facebook_virus_attacks_continues_check_kirgoat_nutpicat_and_brungaat_continue_lure_unwary">Facebook virus attacks continues: Check kirgo.at, nutpic.at, and brunga.at continue to lure unwary</a></li>
<li><a href="http://morisy.com/facebook_says_check_121im_common_sense_says_dont">Facebook says "Check 121.im"; Common sense says don't</a></li>
<li>Facebook's blog post on how to <a href="http://blog.facebook.com/blog.php?post=81474932130">Protect Yourself Against Phishing</a></li>
</ul>
