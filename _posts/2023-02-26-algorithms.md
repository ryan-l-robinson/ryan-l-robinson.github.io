---
title: 'On Algorithms and Section 230'
date: '2023-02-26T08:18:09-05:00'
author: 'Ryan Robinson'
layout: post
permalink: /algorithms-section-230/
categories:
    - 'General Tech Tools'
---


For those paying attention, there are a couple big cases in front of the US Supreme Court that could shape the Internet as we know it. I'm Canadian, but the (English) Internet is largely determined by what is allowed in the U.S., so yes, I'm still talking about it.

## Context

Essentially, the plaintiffs want to hold Google legally responsible that its recommendation algorithm sometimes promotes ISIS recruitment videos. The concept could apply to other harmful content as well.

There is no question that Google is protected in the harmful videos existing on YouTube. It would be impossible for the modern Internet to exist if every piece of content had to be moderated and considered by a team of lawyers before it could go online. That is clearly covered by section 230. 

It's the recommendation algorithm that complicates things, because that gives an impression of an endorsement from Google. Google claims they are protected under section 230, which says they are not responsible for content posted by users and the algorithm's results is effecctively user-generated. The plaintiffs say that Google is not protected because the algorithm for recommendations means Google is acting as a publisher.

[Legal Eagle provides a good breakdown on Nebula](https://nebula.tv/videos/legaleagle-this-supreme-court-case-will-destroy-the-internet) or (appropriately) [YouTube](https://www.youtube.com/watch?v=hzNo5lZCq5M). 

<iframe width="560" height="315" src="https://www.youtube.com/embed/hzNo5lZCq5M" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" allowfullscreen></iframe>

He does a great job explaining why it would be terrible to remove section 230 entirely. The Internet would divide into either no moderation or extremely strict and expensive moderation. So let's rule out that extreme immediately.

But here's where it gets really interesting to me. If not the status quo, and not the opposite extreme, what else is possible in between?

Another distinction he mentions that SCOTUS may try to make is that between recommendation engines and search results, allowing the latter but making the platform provider responsible for the former. He says this would be less of a disaster, but there isn't that big of a philosophical difference between the two, so it might be hard to hold up.

## Personalization

Another distinction even more interesting to me, that he doesn't mention, is *personalized* recommendations and search result algorithms.

### The Impact on the Business Model

This might seem like a smaller change but it hits at the heart of big tech.

The basic business of most big tech is this:

1. They make most of their money by selling ads
2. Ads are more effective if they are personalized
3. In order to personalize, they need you to give them lots of data about yourself
4. The best way for them to get you to give up lots of data is for them to keep feeding you things that you want to engage with

If the recommendations and/or search results were not personalized, you probably spend less time on their service and give them less data. They can still sell ads, but they won't be as effective and they make less money. The big established platforms could still make a profit, I'm sure, but it would be a radical shake up of the entire business model.

### The Impact on Privacy

In terms of privacy, this would be good for users. There would be a lot less incentive for big tech to know everything about us, which could result in unintended consequences like security breaches.

### The Impact on AI Research

In terms of AI, it would significantly slow down development. AI needs lots of data, which big tech already has. If we stop giving as much data, there's a lot less training material. Maybe at this point it wouldn't matter much, since they're already collecting all the data.

## Hate and Progress Movements

What does it mean in terms of social consequences, which is an important question not only because that's related to the cause of the lawsuit in the first place, but also because isn't it really always the big question?

If recommendations and search results were not personalized, they could still be weighted in other ways, like prioritizing content that already has lots of interaction or newer content. It just wouldn't be able to prioritize and give different results based on what the algorithm has determined that you individually will engage with.

That means that everyone sees the same results from the same input. We would lose a lot of the "echo chambers" where you only see things that you want to see, at least not without consciously entering that echo chamber (searching a hashtag, deciding who to follow, etc.)

There wouldn't be an algorithmic push to extremes. This applies to all extremes, not just social/political ones. We'd see a lot of content that is broadly palatable to almost everyone. Think of what network TV was like 20 years ago, when each household had one TV so if you wanted viewership you wanted a show that the entire family could watch together. If you watch some of that content now, it will mostly seem boring, because you're used to media that is much more niche targeted to your interests.

The core argument in favour of this kind of approach is that algorithms stop promoting hatred. It would break the very successful business model of right wing grifters who make lots of money by generating lots of engagement spewing hatred and fear. That certainly sounds good.

But that's not the only group that would be impacted. It would also break the reach of anybody else who doesn't already have a critical mass of followers, like activists. You wouldn't hear from those profiting from spreading transphobic lies, but you also wouldn't hear a lot of important work from trans people telling their stories. You'd see less of the crafted manipulation of authoritarians but you'd also see a lot less of those fighting back. Algorithmic social media is often step one in organizing resistance and a big part of that is because in order to keep you there, they give you something that's a little more of what they think you want. So if you express a little interest in anti-racism work, it's going to help you find more anti-racism, which is great.

This is the area that is the most complicated. Do you consider that a fair trade, even if it were practically possible? And it is also ideological, not only practical: is that a level of regulation that you want your governments to be able to exert - not stifling free speech, but stifling reach?

### Smaller Sites

These kinds of proposals will have 95% of the conversation focused on big tech, but if the rule is established for YouTube, it would apply for everybody else, too.

My day job is for a university library, primarily the website. There is currently no recommendation interface. There are search results, which are not at all personalized, but I've had the serious thought that maybe they should be in a very minimal way. There's a lot of content on the site and a lot of it using similar keywords around databases and resources and citations, so if you use keywords like that, you get a bunch of different pages spanning all of the subjects, likely burying the results most relevant to you. Even one piece of personalized information would really improve search results: what subjects are you studying? Wouldn't the search be better if we knew that and prioritized responses accordingly, giving computer science results first if you're a computer science student?

That's a small example. It doesn't require big machine learning algorithms monitoring your every move on the Internet, but it does still require personalization. Maybe that's the distinction instead: allow personalized results based on information explicitly given by the user, but don't allow engagement data mining. But who defines what is engagement data mining and what is essential information to provide the service, or engagement data mining for telemetry, for the developers to know what improvements they need to maks? My example may have a clearer line, but that certainly won't always be the case.

## Conclusion

There are a lot of complicated factors here and I'm thankful for channels like Legal Eagle that are helping to unpack the potential consequences. Let's hope SCOTUS thinks this through carefully and rules in the best interests of a healthy role for the Internet in society.