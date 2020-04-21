---
layout: post
title: 'PoBoy Twitter Tracker 0.1: A small Python script to collect follower counts'
created: 1269800489
---
<span class="inline inline-right"><a href="http://www.flickr.com/photos/carrotcreative/2511539541/"><img src="http://morisy.com/files/images/twitterbird.jpg" alt="" title=""  class="image image-_original " width="304" height="467" /></a></span>At work, one of the things I have to do is keep tabs on a number of our Twitter accounts. Nothing spectacular, but with 50-ish accounts to keep track of, it gets to be a lot of overhead. So I automated it!

The following Python script simply reads through a text file to find out the Twitter accounts you want to check, and then spits back those account names and how many followers each of those accounts has:

<code>import  csv, math, time
import twitter as twitterapi

#pwd='***'
#api = twitterapi.Api(username='fakeymcfakester', password=pwd)

listofnames = file('twitterusers.txt').readlines()
listofnames = [name.strip() for name in listofnames]

csvfile=open('twittercounts.csv','ab')
csvout=csv.writer(csvfile,dialect='excel')

for name in listofnames:
    account = api.GetUser(name)
    followers = account.followers_count
    print name + ", " + str(followers)
    csvout.writerow([name, followers])

csvfile.close()
</code>

Note that this script requires the <a href="http://code.google.com/p/python-twitter/">Python Twitter wrapper</a>, although it just barely taps into that wrapper's functionality (Note that the script doesn't even require a username or password to work!).

To run it, after installing the Python Twitter wrapper, put the script and a plain text file with the usernames you want to scan (one per line, no commas) into the same directory. Note that right now, there is no error checking, so if one of the usernames is mistyped, is deleted or changed, the script will probably crash. I plan on fixing this in the next release.

It's fairly trivial to expand the functionality to include the number of people that user is following, the latest updates, etc., and for that I highly recommend Amy Iris' <a href="http://blog.amyiris.com/2009/02/get-to-know-your-followers-on-twitter.html">tutorial on Twitter tracking in Python</a>; I simply needed something a little more basic and that output into an Excel-compatible file.
