---
title: Future of Microblogging Social Media
date: 2023-07-14T08:18:09-05:00
author: Ryan Robinson
layout: post
permalink: /future-microblogging/
categories:
  - General Tech Tools
lastmod: 2023-07-15T22:52:12.779Z
---

Twitter, Mastodon, Calckey, Bluesky, Threads... And a whole bunch more that aren't even worth mentioning in my opinion ([I did try a couple of them](/twitter-mastodon-counter-social/)). It's an interesting time for social media, especially the microblogging format.

Part of what makes it so interesting is that there are real differences in philosophies of what the Internet - and therefore, society at large - should be, not only a difference in which billionaire gets to sell all our data.

So, after a particularly tumultous week, I decided now is a good time to check in with how I feel about the current options and where I see things going from here.

## Twitter

Twitter is dying. It may not fully shut down, but there's no trust of anything you read, there's lots of harassment, you're limited in how much you can even use it, there's lots of security failures and privacy violations, occasionally it goes down for several hours. [They're even now bribing far right influencers to keep people around spewing hate speech](https://www.washingtonpost.com/technology/2023/07/13/twitter-creators-payments-right-wing/) so yeah, if you're still viewing Twitter, or still buying ads on Twitter, you're directly funding hate speech.

It's on life support and it's hard to see it lasting for much longer as anything more than Musk's vanity project.

## Threads

Threads from Meta is the other big corporate player, trying to claim that spot as the default microblogging platform. One big difference is that they want it to be more of a happy fun place that advertisers want to be with minimal moderation efforts required, so they're downplaying talk of real life issues.

I have not personally used it. I don't use anything owned by Meta. From what I've heard, it's a very rough start in terms of features, but as you expect from Meta's expertise, it's easy to get started and it got a huge start from brands, journalists, and influencers - the kinds that drive the network effect - in addition to everybody else. The feed is heavily algorithmic, forcefeeding you a lot of brand content instead of who you follow.

Where it gets really interesting is their promise that it will be federated with the ActivityPub protocol, meaning it will not be a complete walled garden. Why are they doing that is hard to say. Maybe they think it will appease regulators. Maybe some engineer who does believe in federation proposed it without really thinking it would be approved and it got through. In any event, it's great to see. I'll respond to more of that below.

## Bluesky

Bluesky is the most interesting, somewhere in the middle of the spectrum. It's federated, sort of. They're promising their protocol will be available to others. But it isn't yet. And it's a unique protocol, not tying in to ActivityPub, the established standard. Which means is still exists on its own, like Twitter, at least until the protocol is done and they manage to sell others on it.

In my time there, I've struggled to see a unique selling proposition that can keep it going. It has some nice features: the options for content filters, being able to subscribe to someone else's mute list which can shut down problem accounts faster, making your username a domain you own, some degree of customizing your feeds. But as I learned back in the Google+ days, features alone do not a social network make, especially once the established players start copying the best ideas.

The unique selling proposition so far seems to be that it is not as much of a cesspool as Twitter, not as confusing to sign up as Mastodon, and not controlled by an evil megacorp like Threads. That comes from the exclusivity of being invite only at this point: most of the people who are there are more or less on the same page with what they want from this network.

But the seams are showing with each time it fails to moderate well - they don't even have a trust and safety leadership structure - and as the user base steadily grows. As eventually happened with Facebook, exclusivity isn't much of a selling point when it will get more inclusive over time. Facebook survived because there wasn't much in the way of competition. But for Bluesky? There's plenty fighting for this space right now.

And more to the point, most of the people I see there I don't think really want exclusivity forever. A lot are socially conscious "shitposters" and journalists and authors. I was for a while referring to the first group mostly as activists, but I've realized that isn't quite right. They're more like we saw a lot on Twitter, people who compete for the most snarky response to whatever the story of the day is that we're all angry about, then move on to the next thing tomorrow. That's not so much real activism, who are usually more focused on long-term efforts toward a specific cause.

But in any case, wherever it falls in the real activism work vs shitposting spectrum, it can only go so far in a closed bubble. Most of them are still on Twitter and/or on Threads as well for that reason. So how long do they want to spend also focusing efforts on Bluesky? Or do they keep it as their secondary place of rest, to recover from the more frontline work elsewhere?

I see that fading out as the exclusivity fades and the lack of trust and safety becomes more obvious, and I'm not sure they'll have any other selling point to replace it. Bluesky seems to think the selling point is their protocol, but it's not even done yet and most people don't care about federation. Those who do are already in the fediverse.

Maybe I'm wrong. Maybe they hire a big moderation team that sets the new gold standard for protecting marginalized people. That would certainly be a selling point. But they aren't doing that so far and that makes me think they don't have much of a future.

## The Open Fediverse: Mastodon and Calckey

Mastodon is where I have mostly found my home (@<Ryan@mstdn.ca>). It's got years of stability in its extensive features - some would argue too many features that make it harder to use. It's on the ActivityPub protocol so it connects with other fediverse projects, including eventually Threads. The complaints are mostly that it is hard to use, especially signing up and having to pick a server.

Calckey is another in the fediverse that addresses some of the concerns many have with Mastodon, like full text search and quote posts.

There are lots more that I won't get into: Pixelfed for photos (think Instagram), Bookwyrm for book reviews (think Goodreads), Lemmy or Kbin for more forum-like conversations (Reddit)@. They can all talk to each other. That's a pretty promising future.

## Predicting the Future

My guess of what happens is we end up like email. A few big corporate giants control most of the email: Google, Microsoft, etc. They offer the service for free in exchange for mining data and showing ads, or in some cases also with a subscription offer that doesn't show ads for a monthly fee (Microsoft 365 Home includes this). It's a quality service, with many professionals working on problems like spam prevention and security patching. That's likely to be Threads the way things are currently going.

But it is possible to run your own email server that can send messages to and receive messages from the big ones or other small email servers. It's not easy. You'll have to meet some fairly high security standards and spam prevention. But you can. That's a lot of the smaller cases of people running their own Mastodon or other servers for a few dollars a month.

Or you can pay for a professional version of email, like Microsoft 365 Business. There's no ad scrapings, they'll take care of most of the security and maintenance, and you just need to pay a few dollars a month and configure it to your liking. That's a great option if you can afford it. In this comparison, that might be some of the bigger fediverse instances. Most of them operate on a donation basis. You don't have to support them financially, but somebody does have to or it won't keep going.

I suspect that's where we get with microblogging, and I'll consider that a huge win. Threads may be the equivalent of Gmail, that many have. Most people will still opt for giving all their data to a billionaire for the right to look at ads, in exchange for all the ease of use that a company like Meta or Google can provide. But you will have some choice other than that and being a hermit, an option that has been increasingly tempting for me over the last 10 years. Maybe you host your own ActivityPub service. Maybe you pay somebody else. Maybe they implement ads but without the data mining. Maybe you stay on somebody else's without ever giving back or seeing ads. But I am happy that at least in this future there would be options.
