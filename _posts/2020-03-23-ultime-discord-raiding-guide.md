---
layout: post
title: "The ultimate guide for raiding Discords."
excerpt: "A little party never killed nobody 😏"
categories: [tutorial, discord, python]
comments: true
image:
  feature: https://images.unsplash.com/photo-1444703686981-a3abbc4d4fe3?crop=entropy&dpr=2&fit=crop&fm=jpg&h=475&ixjsv=2.1.0&ixlib=rb-0.3.5&q=50&w=1250
  credit:
  creditlink: 
---

Have you ever had the sudden urge to spam the heck out of a discord server? ***Never?***<br>
I'm pretty sure I'm not the only one, since most of the servers I'm at have suffered a lot of these famous "raids". I've even done some... 😉
<br>
For those who don't know what they are, they consist of people joining random Discord servers and just spamming `@everyone` or `@here`. Seems like something pretty simple to do, it's just joining servers, but things start getting funnier when they think you're a hacker just because you are bypassing their bans.

Obviously, you cannot bypass a ban *(unless you're taking advantage of a vulnerability in Discord)*. Then, how do you keep joining a server even after they banned you? You guessed it: *alt accounts*.<br>
Alt accounts, or just **alts**, are multiple accounts that are owned by the same person.<br>
Yeah, I know, creating multiple emails, and then a discord account each time you get banned, might be really annoying.<br>
Plot twist: what if I told you, you don't need to create multiple emails, and that there's a simple python script that can create thousands of accounts, with just 1 email?<br>
Now things are getting more interesting...

<div markdown="0"><p style="color: red;"><b>This article's purpose is just educational. It simply exposes some of Discord's problems when it comes to account creation and how a simple python script can easily create thousands of accounts with just 1 email.</b><br>I'm not responsible of whatever you do with this.</p></div>

This article assumes a prior knowledge of:
- Git
- Python

If you know all of these things, let's start!

## Installing DiscordAlt
DiscordAlt is a CLI tool that will allow us to create multiple accounts with the same email. It is exactly what we need, and is what we'll be using.<br>
Installing DiscordAlt is a pretty straight-forward process, all you need to do is run the following commands:

{% highlight bash %}
git clone https://github.com/DiscordAlt/DiscordAlt.git
cd DiscordAlt
./init
{% endhighlight %}

> If you get `permission denied: ./init`, it is just a permissions error. Fix it by running `chmod +x ./init`.

This script will prompt for your an email, which will be used for creating the alts; and your Discord username, which will be used for retrieving the profile picture, and social-links, for making the alts look more realistic.<br>
Once you entered all the necessary information, you'll be prompted for the number of alts you want to create.
Once all the alts are created (you'll know when because you'll see a green message saying "<b style="color: lightgreen">Discord alts created succesfully</b>"), you will need to enter a text. This is what your alts will be saying once they join a server.<br>
After all entering all the information, **i promise this is the last thing**, you'll be asked for a discord invitation link, which is what the alts will be using for joining the server.

Once done this, you'll see a nice command line interface. If you type `help`, you'll see all the available commands, but, as everything is configured, you'll just need to enter the following command:
{% highlight bash %}
raid -r config.txt
{% endhighlight %}

**And Viola!** Your bots will now be joining the discord server and start spamming messages!<br>
Don't you love it when you see how an entire army of 200 alts join a server and spam `@everyone`?