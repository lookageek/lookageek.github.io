---
layout: post
title: being simple when you program
date: 2016-01-11
summary: simple is awesome
---

I was a novice Java Developer doing a Web API for my startup — with having no clue on coding patterns and designs to build a codebase which can evolve gracefully as it would hit shore after shore of change in the days to come.


To think of the irresponsibility involved, that codebase would definitely tick off every item in a “no-no” checklist of an experienced developer’s mind.


But then, I have hurriedly left my startup some time back. That story ends there.


I joined as a Rails developer involving an early-stage product development.


As I moved from Java to Ruby — I seem to have noticed, absorbed and inculcated a treasure trove of ideologies and mindsets that Ruby community and Object Oriented programming community have been teaching for years.


Interestingly enough, I wasn’t naturally exposed to any of it when I was working with Java — an OO language. Maybe I just did not stumble upon them at all. Just a personal opinion. Please don’t grind any axes. :)


Very prominent among them for me is *__simplicity in crafting software__*.


---
*__“simplicity is complicated”__*


This phenomenal [talk by Rob Pike](https://www.youtube.com/watch?v=rFejpH_tAHM), creator of Go was the primary reason that this post is here — i got pushed to condense all the ideas I have come across until now.


Aiming for simplicity in code cutting the cruft will lead to a state of zen in your codebase — a tiny effort required to battle any storm of change that may come tomorrow, because change, as we all know — is the only constant!


Simplicity’s sibling — Orthogonality is that quality that creates reusable pieces and parts of code that solve one thing, and solve it really well and be rock-solid dependable!


Hitting orthogonality in code strikes off ‘O’ in SOLID too — Open/Closed principle. Such a setup is open for adding a new piece and mixing it up with the existing code for extension, but closed as you never need to touch the existing code.


But this orthogonality is hard to get by. So is simplicity.


Adding cruft, bells and whistles to code may become a natural tendency. The elephant in the room to address is to not stare at the code! Instead, it is the mindset of trying to foresee the future getting it done now itself rather than doing what we need today and doing just that really well.


The mantra to great orthogonality may lie in very good hindsight in separating concerns. This may not be immediately apparent today when you are developing this thing you have at hand. That’s okay. As I will discuss soon, always be refactoring towards it!


It’s a continuum towards orthogonality — not a binary state, and you should know where to stop too avoiding ‘over-engineering’!


---
*__simple code is testable__*


Now an obvious side effect of such a code — with no rabbit holes is that you get to test your code with not much head-banging. Not a lot of mocking, stubbing and data setup needed: since simplicity. Not a lot of expectations to write to test the same piece: since orthogonality.


Converse also applies, if you are doing too much to test something, it is not there yet and it will cause you pain… So go refactor!


---
*__“always be refactoring”__*


Naturally, it leads us to this.


These blog posts — [here](https://robots.thoughtbot.com/how-much-should-i-refactor) and [here](https://robots.thoughtbot.com/refactor-until-you-feel-almost-comfortable) from [thoughtbot](https://robots.thoughtbot.com) have already have given due diligence. I will be just presenting an abstract condensation of my novice perspective.


Change is the only constant in software lifecycle and new knowledge today about our product / project will lead us down paths we could have never dreamt of in the past. Top it with the fact that such codebases will thrive out in the world for a long time — witnessing a sea change every passing day!


If one sits at the desk ferreting the change to the code without pragmatically utilizing the new knowledge to the full extent — surely soon we will be left with a towering mess that has so much resistance and threshold energy against the change that has to be bulldozed down. Quite dystopic!


Utilize what you learnt — the new knowledge. Refactoring is a continuum! Only that will lead to maintainable code!


---
*__“duplication is better than incorrect abstraction”__*


Alas a word of caution! This quote from [Sandi Metz](http://www.sandimetz.com/) comes to my mind.


Abstraction hides a complex implementation and gives a layer of clean interface to anyone who wants a task done. Abstraction, just like Orthogonality makes the codebase ready to go down any path in future.


But abstraction made by utilizing less knowledge may be an incorrect one! And will bring down ease of change because an incorrect abstraction will bear the brunt when the spec changes and may need to be torn down as well.


So if you are not convinced that abstraction is required right now, keep the duplicate logic. Just don’t meddle with it yet. Time will come!

Well that’s it for now!
