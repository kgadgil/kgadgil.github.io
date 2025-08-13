---
layout: page
title: Tsundoku or Cozy Bookstore
summary : PWA idle game in which you collect books
date: 2025-08-12
---

[🔗 View the full project on GitHub](https://github.com/kgadgil/cozy-bookstore)

---

# Tsundoku: The Book Collecting Game I Didn’t Know I Needed

I was in bed, winding down for the night, when I borrowed an audiobook from my local library. My plan: listen to a story for an hour, drift into sleep, maybe dream something cozy. The book was called *The Full Moon Coffee Shop*.

Within the first ten minutes, the main character introduced herself as a scriptwriter for mobile games—and my brain immediately latched onto that.

That morning, I’d clicked on an ad for a game called *King Shot*. I’ve recently fallen down the rabbit hole of idle games—those easy, background-friendly time sinks where you build castles, farm vegetables, and collect resources while barely lifting a finger. So naturally, I’d searched “Idle Games” on the Play Store to see what else was out there.

Turns out, there’s an idle game for just about everything: mining, banking, lording over vassals (yes, I typo’d it as “vasslaa” in my notes), distilling whiskey, running lumber yards, managing coffee shops and boba tea stands… even dinosaurs, hotels, and prisons.

And yet, when I looked for a *bookstore* idle game—nothing. No game that let me collect books.

I gave up my search and, instead of sleeping, decided to see if anyone had actually researched idle games. Scholar search did not disappoint. I found two papers:

* One that categorized idle games into four main types (none of which I played) and introduced me to the “OG” clicker, *Cow Clicker*. [1]
* Another on *Neko Atsume*, the cat-collecting game that charmed half the internet. [2]

Somewhere between *Cow Clicker* and *Neko Atsume*, the idea hit me: a **book collection idle game**.

At this point, the plan to “listen and drift to sleep” was long gone.

---

## From idea to app in a single sitting

I could’ve kept researching game mechanics, but instead, I decided to run the idea past GPT. It gave me a few charming sketches—one included a cat curled up in the corner—that I could immediately picture. If I had front-end or artistic skills, it could’ve looked beautiful.

I didn’t.

So I went for something I *could* do: a simple Progressive Web App in basic JavaScript, easy for me to debug and maintain. I moved from bed to desk, laptop open, and a few hours later, I had a working prototype live on GitHub Pages.

It wasn’t fancy. But it was playable.

I even threw in small touches, like a toast emoji popping up when you gathered bookmarks.

And here’s the thing: I was actually having fun—both coding it and playing it. This little project reminded me that I can entertain myself, not just by coding, but by coding up apps *only I* would want to play.

---

## Naming it, living with it, loving it

I’m still in the “user testing” phase (read: playing it myself for days now). My main feedback so far is catalog-related, and I want to add a feature that lets me tap through to Goodreads or Google Books for any title I collect.

As for the name, I briefly considered “libarchive” as an inside joke—since I’ve been working with the actual libarchive library for over a year. But then I thought of *Tsundoku*: the Japanese word for acquiring books you don’t necessarily read, but keep around because they feel like friends.

That meaning hits close right now. I recently gave away about 200 books when I moved countries, and I’m not ready to buy new ones yet. There’s a guilt to owning unread books, but also a deep comfort in being surrounded by them. This little virtual bookshelf scratches both itches.

---

## The game loop

At first, I set the “book drop” timer to just a few minutes for testing. Then I remembered *Cow Clicker* drops coins every six hours, so I settled on a one-hour book drop. You can earn upgrades, force deliveries, and—like me—you’ll probably check the app a few times a day to see what’s new.

Just yesterday, I “collected” *The Sound of a Wild Snail Eating*—a memoir about chronic illness and the companionship of a snail. It’s exactly the kind of delightful, random find that makes tsundoku so irresistible.

---

I don’t know if anyone else will play this game. I don’t even know if I’ll polish it up enough to release publicly. But I do know that building it brought me joy—and that’s a pretty great metric for success.


References:
[1] Alharthi, Sultan A., et al. "Playing to wait: A taxonomy of idle games." Proceedings of the 2018 CHI Conference on Human Factors in Computing Systems. 2018

[2] Cutting, Joe, David Gundry, and Paul Cairns. "Busy doing nothing? What do players do in idle games?." International journal of human-computer studies 122 (2019): 133-144.