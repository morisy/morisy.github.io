---
layout: post
title: 'Some tips on using OpenHeatMap: A survivor''s tale'
created: 1292315962
---
I have now spent a long, long time getting acquainted with the wonderful <a href="http://www.openheatmap.com">OpenHeatMap</a>, a delightful project by <a href="http://petewarden.typepad.com/">Pete Warden</a> that easily lets you map your data sets against not only maps (as the name would apply) but also time. 

If you use the website's "hosted version," the whole thing is a snap. Just upload your CSV or Excel document, or link in a Google spreadsheet, tweak a few knobs, and you are off and running. If you want to host it yourself, however ... There's a few speed bumps along the way. And as far as I can tell, no one outside of Pete and myself has really done it yet.

Now first off, Pete's done a great job and the <a href="https://github.com/petewarden/openheatmap/wiki/">Github documentation</a> is pretty good given the project's infancy. But I banged my head on a lot of points that hopefully others can avoid, because I couldn't find any non-Pete written documentation or reviews anywhere.

So here we go: Michael's caveats and warnings when using OpenHeatMap.
<!--break-->
<b>1. Take the warning about cross domain problems very seriously</b>

<a href="https://github.com/petewarden/openheatmap/wiki/How-to-use-OpenHeatMap-within-your-own-site">From the documentation</a>:
<blockquote>Because the rendering code is held on the openheatmap.com server, you will need to grant cross-domain access if you want to allow it to read the CSV files from your own server. You can download mine from http://www.openheatmap.com/crossdomain.xml or here’s the contents of a crossdomain.xml file to enable that, you’ll need to save it in the root folder of your webserver:

<?xml version="1.0"?> <!DOCTYPE cross-domain-policy SYSTEM "http://www.macromedia.com/xml/dtds/cross-domain-policy.dtd"> <cross-domain-policy> <allow-access-from domain="static.openheatmap.com" /> <allow-access-from domain="static.openheatmap.com.s3.amazonaws.com" />

As an alternative, you can copy the http://static.openheatmap.com/openheatmap.swf file over to your local server, and supply your local URL as the optional fourth argument to insertOpenHeatMapInto(). If you take that route you won’t get automatically get updates and bug fixes to the rendering component, and you may want to copy over the openheatmap.js file also to ensure everything you need is local.</blockquote>
I went with the latter route for better portability, but configuring OpenHeatMap to call my SWF, and not Pete's hosted version, took me a lot longer than it should have.

This is the code that ended up working:
<script src="http://pastebin.com/embed_js.php?i=584pBjF6"></script>
There are a few alternatives sprinkled throughout the documentation, but none of them worked for me.

<b>2. Some stuff only works on a server</b>

I'm too tired to understand why, but I banged by head for hours on the local version and was about to file a ticket with Pete. So I uploaded my non-working code to the server and - voila! - it started working. Partially. Well, at least good enough to let me figure out some next steps.

<b>3. Pete Warden is sneaky</b>

I slogged through the documentation several times, but since the included Hello World example didn't work (see above) I had to look through the examples posted on the OpenHeatMap site. A few of them were very similar to the effect I wanted, which was an interactive timeline that I could press play or scroll through manually. But when I looked at the source, none of the variables I was hoping to reference were there. For example, I couldn't get the time bar widget to load, so even though I defined a start and end date, there was no way to cycle through the years I was tracking.

Turns out, Pete stores all this stuff in separate JSON files that are semi-hidden away, but what I did was use his wizard to create a map similar to the one I wanted, and then note the three-word code above it. Copy and paste that three word code into here:
http://data.openheatmap.com/[THREEWORDCODE]/map_settings.jsonp
Then you can see the exact longitude and latitude of the view you like, that ""has_time":true," is what you need to add in a timeline, and much, much more. You'll have to fudge around with the formatting, but at least it gives you a sense of how the variables are used and can cut out some nasty back and forth tweak-upload-view-repeat cycles. 

Overall, OpenHeatMap is great, but it could use a lot more example files and some clearer explanation getting it up and running locally. If you've had problems, leave them in the comments and I'll try and address them, but overall, this is a great project and provides a nice alternative to Google Maps/Google Fusion Tables that lets you keep control of the data.

Thanks Pete!
