---
title: Getting Lost, Algorithmically
---

I recently noticed that when I go for a walk, I always end up going down the same routes. With a desire for finding a new and potentially exciting area to explore I decided to get lost. But 'getting lost' was a little bit too vague for my liking. How would I achieve that?

So I came up with a set of rules that would result in me getting lost. Whenever I would come across a fork in my path I would take the path that I have taken the least amount of times. This seems like a pretty intuitive way to end up exploring a new area, but as I discovered it is actually flawed.

Firstly, suspend all awe you may have and imagine that this is me walking.

![A pink star with arrows pointing to represent paths](/assets/walkin.PNG)

The arrows are the possible paths I can walk down and the numbers represent the amount of times I have taken that path in the past. So the path with "100" means I have walked down that path 100 times before. Using the rule I previously mentioned I am going to go down the paths 10-100-10 ten times. This is undesireable for 2 reasons. FIrst, I would prefer not to look like an insane person. Secondly, I want to explore new places but the rule just makes me travel a path I have already been to 100 times. So the rule is not ideal.

An easy way to deal with the first problem is to ignore any paths I have already been to on this walk. But it does not solve the second problem, as I will still go down the path I have already been down 100 times.

