---
title: Getting Lost, Algorithmically
---

# {{ post.title }}

I recently noticed that when I go for a walk, I always end up going down the same routes. With a desire for finding a new and potentially exciting area to explore I decided to get lost and explore new places. But 'getting lost' was a little bit too vague for my liking. How could I achieve it?

So I came up with a rule that I hoped would result in me getting lost. Whenever I would come across a fork in my path I would take the path that I have taken the least amount of times. This seems like a pretty intuitive way to end up exploring a new area, but as I discovered it is actually flawed.

Firstly, suspend all awe you may have and imagine that this is me walking.

![A pink star with arrows pointing to represent paths](/assets/walkin.PNG)

The arrows are the possible paths I can walk down and the numbers represent the amount of times I have taken that path in the past. So the path with "100" means I have walked down that path 100 times before. Using the rule I previously mentioned I am going to go down the paths 10-100-10 ten times. This is undesireable for 2 reasons. FIrst, I would prefer not to look like an insane person. Secondly, I want to explore new places but the rule just makes me travel a path I have already been to 100 times. So the rule is not ideal.

An easy way to deal with the first problem is to ignore any paths I have already been to on this walk. But it does not solve the second problem, as I will still go down the path I have already been down 100 times.

A way to combat the problem could be to look at the next, lets say, 3 paths and go down the path with the lowest total familiarity. So in the example above the total 'familiarity' on the left path is 120, and on the right would be 30. It's easy to think of a counter-example though, as we could imagine a scenario where the 4<sup>th</sup> path has been travelled down 100000000000000000 times and the algorithm would not consider it. We could try to increase looking at the next 3 paths to 4, or 5 or some large number such that we would not realistically run into an issue but it does not rule out the possibility which is annoying. Also, as the number of paths we look at increase the more we will have to think about it at each fork in the path and I would prefer to be able to make the decision instantly.

If I give up the first requirement, which was to avoid rewalking down the same path more than once, I can come up with a rule to satisfy the second requirement.

If I 
