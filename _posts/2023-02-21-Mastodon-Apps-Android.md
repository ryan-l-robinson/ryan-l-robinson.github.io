---
title: Mastodon Apps on Android
date: 2023-02-21T08:18:09-05:00
author: Ryan Robinson
layout: post
permalink: /mastodon-apps-android/
categories:
  - General Tech Tools
tags:
  - Mastodon
slug: mastodon-apps-android
keywords:
  - Mastodon
type: default
draft: false
---

I've been enjoying my time on Mastodon since the recent migration from Twitter. Of course, I'm far from the only one to make this migration, and that includes a lot of developers, so we're starting to see a lot of better apps for Mastodon and the wider fediverse popping up. That has led me to an experience that has been very rare since about 2012: testing out and researching a variety of independent apps to meet a need. For years I've mostly just used whatever the official app is for whatever service (including Twitter), with really the only recent exception being when [I spent some time testing out alternative email apps](/android-email-apps/).

Before writing this post, I put the question out on my Mastodon to see what factors others have considered in picking their preferred Android app. I'll incorporate a couple of those answers here, but first, one shared [a very helpful spreadsheet breaking down all the options](https://docs.google.com/spreadsheets/d/1De5KRwqMIdwEryfoeBLARgxF7QgKkeOQBCilKuIdAXE/edit?usp=drivesdk) (not only Android). This is great if you need a high level overview of features available.

This post will try to narrow down some of what matters most to me and to others when I put the question out for feedback.

## Mastodon (official app)

As I'm sure with most people, I first tried the official app simply called Mastodon. This was the time of the great migration and a significant portion of posts I saw were advice about Mastodon, including a lot of posts saying not to use the official app. But it's not as bad as that makes it sound.

It has Trending topics. It has home and local feeds. It's a fairly clean and friendly design.

But yes, as many point out, it is missing several other features that you might want. Check the spreadsheet linked above for the full list, but here are a few that that matter to me:

You can't read threads in continuity, which makes it prone to reading posts without recognizing there's context.

There's no federated timeline.

You can't manage lists at all.

You can't see ALT text, which does matter even for those of us who are sighted because descriptions can still help us identify things, and it might help us identify that maybe we don't want to boost a post that is missing ALT text.

It doesn't support unlisted posts, or scheduled posts, or the delete and redraft option, or simultaneous posting of a thread, or multiple choice selection polls.

It's fair to say that none of those are core features, but there's enough of them that there's probably at least one you'd be disappointed to be missing.

## Tusky

When I was seeing posts about not using the official Mastodon app, it was usually tied with the recommendation to use Tusky instead (sometimes Fedilab). I tried that and kept it as my main app for a couple of months.

It does a few things very well:

- Very clean design that feels at home on Android, especially with the truly black theme and options for the main navigation to be either at the top or bottom
- A good array of options including being able to do most of the things that the official Mastodon app cannot.


My question on Mastodon also got this negative response about some of Tusky's design choices:

> I’ve been a mobile developer for 15 years (mostly android) and used Tusky before I got my iPhone. It wasn’t my favorite tbh. my gripes with Tusky are all around data and state handling.
>For instance the UI has very few “in progress” states, so for instance boosting a toot can  momentarily show the button in the wrong state if the request is slow.
>Also the caching for viewed toots is very rudimentary, so lots of toots (in conversations esp.) are needlessly reloaded while I stare at a blank screen.
> - Source: https://tech.lgbt/@em_ad/109855207946318853


## Fedilab

I then tried Fedilab, the next I saw recommended a lot. It has a small one time cost for the app, but if you're already settled on using Mastodon, it will probably be worth it to you to try it out.

### Positives

As the spreadsheet backs up, it is the most featured app by a significant margin. I'll highlight a couple big selling points that the others don't have:

It allows following other instances, which is a great way to monitor niche topic communities even if you're not in them. For example, there is an instance for Drupal developers at drupal.community. I don't really want that to be my primary home, since Drupal is a relatively small portion of what I post. But I do want to easily keep an eye on conversations happening there since they will have a high rate of being relevant to me.

It allows following Twitter accounts via Nitter, although there are some drawbacks to how it is implemented. You can't edit the list of who you are following easily. There's no follow/unfollow buttons. There isn't even a way to view the list of everyone you currently follow. So you need to maintain a list somewhere else, in the right format (separated by a space, not a new line) so that you can copy and paste it in each time you want to add or delete one. It also may have a limit on how many total it can follow? I'm not sure about that, but I found that when I tried to add more, it broke, with a generic error that didn't explain anything. And finally, a lot of the time the links it shows for a quote tweet simply don't work. I often try clicking the link several times in a row to see what is being quoted.

It allows creating simultaneous posts in a thread, which none of the others do. I always appreciate this feature as I don't like getting caught having written up half a thread. This is even more true on Mastodon than on Twitter because it is best practice to keep all posts in a thread after the first as unlisted. But when there are long gaps between the start and end of the thread, I might end up with nobody even seeing that you have added more to it. Being able to dump the whole thread at once optimizes that best practice.

It is one of the few apps that is built for all Fediverse services, not only Mastodon. That means if I get a Pixelfed account some day, I could do it from the same app.

A Mastodon user highlighted another feature that isn't a big deal to me but might be to you:

> I read the posts from oldest to newest. At the moment Fedilab seems to work best for this reading order, as it can continuously update the timeline so there are no breaks.
Tusky is second best, you can set the "load more" button to fill the timeline above the break, not below.
Still no app seems to allow reverse order timeline (oldest posts first), which was a deal breaker for me when selecting my Twitter app. 
> Source: https://mastodonsweden.se/@kallekn/109856154392108362

### Negatives

Most of my negatives have to do with the user interface and I'll focus on two:

I don't like the pill button design. It feels out of place on Android. It feels dated, like a few years ago when there was a lot less consistency in app design on Android, while now most comply with the recommended design language.

I don't like the fragmented placement of timelines. In the bottom toolbar you can have the home, local, federated, notifications. That's great. Then in the top go any other instances you follow, lists, and Nitter, in this weird ticker style interface. Then in the sidebar under the profile photo mostly makes sense but also has Trending in there. I'd love to have these consolidated to one navigation area, in the bottom, where I can pick the four that are highest priority to stay with easy access, then the rest in an easy to access overflow menu. There is an option to combine the top and bottom, but only to put them all in that weird top ticker style, not in the bottom as I would want. And there's no option to add Trending there.

## Megalodon

This is the newest discovery for me. It is not heavily featured - a little more than the official Mastodon app, less than the others - but it looks fantastic, probably my favourite design of the bunch.

## Conclusion

For now, I'm sticking with Fedilab. I really like some of those features it does better than the rest, enough that I'm willing to sacrifice some annoyance at the design style. But I am going to keep the others around and check in on them occasionally. It's early enough in the life of most of these that they may catch up in the features while maintaining a nicer design.