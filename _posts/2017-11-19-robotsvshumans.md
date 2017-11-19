---
layout: post
title:  "Robots vs Humans"
date:   2017-11-19 15:30:00 +0200
categories: blog
image: "../assets/blog3.PNG"
---

robots.txt is a file that you place in the top-level directory of your web server. The text file contains instructions to robots, for example search engines, about which folders and files they are not allowed to access. However, this is not like a firewall - bad robots can choose to not even look at your robots.txt file and still access the files you don't want them to access.

My robots.txt is configured so that search engines will not index my blog posts or the images I upload. But they are allowed to access my index page and the page that's about me. This was done by writing the following:  
{% highlight ruby %}
  User-agent: *
  Disallow: /blog/
  Disallow: /assets/
{% endhighlight %}

### humans.txt
humans.txt is a file that contains information about the author of the website. You're not required to have a humans.txt on your web server.
I've configured my humans.txt to present information about me as a developer/web designer. I also present some information about the website and the tools used to develop the website. This is what it looks like:  
{% highlight ruby %}
  /* TEAM */
  Developer/Web designer: David Sjögren
  Contact: sdavid2304@gmail.com
  From: Kalmar, Sweden

  /* Thanks */
  Lecturer/Examinator: Johan Leitet

  /* Site */
  Last update: 2017/11/19
  Standards: HTML5
  Software: Jekyll

{% endhighlight %}