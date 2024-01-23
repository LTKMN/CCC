# CCC
Cute Courier Club, a game for biking around town

I'll update this just so I don't forget:

the general idea was a game that runs in your mobile browser (or otherwise built in a language that supports both android and iOS - I don't _care_, I just want both) where you give it GPS permissions and it takes where you currently are and sends you on a quest to a random valid street location within a set radius. you IRL bike there, and it gives you little rewards for doing it.

basically it's strava roulette - we like biking in the summer but we never really know where to go, so having a quest-giver roll something for us is fun.

and then in my head it had a little cast of animal crossing-like characters who would pop up and do some talking, maybe the trip is couched in a sort of courier role where you have to deliver a macguffin to another character and they give you a prize in return. the rewards are arbitrary and adorable, etc.

then your strava bragging is actually just having a virtual shelf of these .pngs of baked goods and tchotchkes that represent distance and deliveries made. maybe there's unique ones with special goals (did it while raining, did it after dark, did it with a friend, etc) and seasonal things depending on how elaborate you want to get.

there is [a netlify pointed at this repo](https://main--papaya-cobbler-62edd4.netlify.app/), but it only works on browsers that actually have GPS access - my desktop doesn't display anything


* * * * *

as it stands there is exactly one index.html that pulls a JS map library called leaflet, and it does the 'find your position' + 'find a random valid position' thing on page load. so even in this state I guess technically it would be functional for my personal goals, but obviously it's not really a _game_ yet.

things to do at minimum:

- wrap everything in a UX that isn't just a blank website with a map frame
- allow setting of an arbitrary trip distance, such that you can choose your level of biking difficulty
- allow re-rolls
- some sort of success when you register your GPS making it to that point
- log it as a running high score?
- some error state pages and things for desktop, etc.

things beyond that:

- my plan honestly was just to generate a library of character portraits and items using AI such that I'm not spending a million years making assets that are basically arbitrary
- make or find a little dialogue system that pops up a portrait and spits out some strings in a nice little speech balloon
-   (and then, I guess, have a list of strings to pull from)
- the success screen would have another recipient character portrait and some gratitude remarks to pull from, then "hands you" an item which has a little toast with some stars and fireworks and whatever
- log that item into an inventory / cookie?
- have a scrolling shelf that displays all your rewards (I'm imagining the old skeuomorphic apple books app shelf)
- whatever else it morphs into along the way
