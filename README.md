## Welcome to Hoo
#### A Playground Agent Based Model Repository

[Placeholder for a cute Owl (named Hoo?) who is the (so far, invisible) mascot for this project]

1. [Intro to `Hoo`](https://github.com/emmagras/hoo-will-build-the-roads/blob/master/README.md#introduction)
2. [Intro to *Agent Based Modeling*](https://github.com/emmagras/hoo-will-build-the-roads/blob/master/README.md#what-is-agent-based-modeling)
3. [Cases to Explore](https://github.com/emmagras/hoo-will-build-the-roads/blob/master/README.md#cases)
3. [Dependencies](https://github.com/emmagras/hoo-will-build-the-roads/blob/master/README.md#dependencies)

### Introduction
###### (Skip to [Into to Agent Based Modeling](https://github.com/emmagras/hoo-will-build-the-roads/blob/master/README.md#what-is-agent-based-modeling),    [Back to top](https://github.com/emmagras/hoo-will-build-the-roads/blob/master/README.md#welcome-to-hoo))
My main desire in this project is to give my frustrated Northern Virginia commuter thoughts some outlet.
I like to imagine what the world will be like when cars can drive themselves, but there are quite a number of roadway institutions to choose from regarding how traffic flows in a more automated world. While we can't be certain we'll ever find the global maximum, we can use agent based modeling to explore a number of the imaginable frameworks and seek to understand the set of local maxima possible within each.

### What is Agent Based Modeling?
###### (Skip to [Cases](https://github.com/emmagras/hoo-will-build-the-roads/blob/master/README.md#cases),  [Back to top](https://github.com/emmagras/hoo-will-build-the-roads/blob/master/README.md#welcome-to-hoo))
Agent based modeling is a simulation technique where the simulator creates a number of autonomous `agents` who can interact with each other in various ways. Typically the agents have a number of parameters that can be altered to study the impact of different variables in the system. 

In this project, the agents are, for the most part, cars on a road. Each car is an instance of an object which has a speed, a direction, and a location. We can then, for instance give each car a `following_distance` parameter and study the effects on traffic of increasing or decreasing. 

Without careful forethought, it's always possible to make ineffective policy decision in the name of good or progress. Agent Based Models help provide visible examples to counterintuitive tendencies, like [Braess' paradox](https://en.wikipedia.org/wiki/Braess%27_paradox) which explains that **adding a road to a congested road traffic network could increase overall journey time.** This project will use game theory and Python's Agent Based and statistical modelling capabilities to test hypotheses about how we can best construct our future roads.

### Cases
###### (Skip to [Dependencies](https://github.com/emmagras/hoo-will-build-the-roads/blob/master/README.md#dependencies),  [Back to top](https://github.com/emmagras/hoo-will-build-the-roads/blob/master/README.md#welcome-to-hoo))
These cases can be vague, and readers are invited to contribute. Exploring cases with a well reasoned theory behind it is important, but half of the point here is to have fun. 

Each of these case studies can be parameterized with varying agent population sizes and densities, ratios of autonomous to non-autonomous cars on the road, and the configuration of the roads. 

1. 
  - Question:
    - Can a minority of autonomous cars on the road respond to traffic patterns such that they break up traffic jams?

2. 
  - Question: 
    - What can we do about non-autonomous cars and pedestrians who abuse the overly cautious safety features of autonomous driving
  - Considerations:
    - Costly punishment (I spend `X` dollars to steal `p*X` (such that `0<p<1`) from you as punishment
    - Toll roads with increased costs for non-autonomous cars in certain lanes

3. 
  - Question: 
    - What are the various speed regulation rules on the road. What implications do they have on cars with smaller spending potentials, or even nearby real estate
  - Considerations:
    - Marginal cost of driving as a function of the lane a car is in, how fast, its size, etc
    - Cars bid for space on the road, pay other cars to move out of the way
    - What happens w/ accessibility to real estate in a busy area (for example if cars bid for traffic signals to change and homeowners can't costlessly get out of their neighborhood) 

### Dependencies
This project is being written in and only supported for Python 3. 
Some of the possible dependencies are: 
- python3
- [Shapely](https://github.com/Toblerity/Shapely)
  - `sudo pip3 install shapely
  - Libgeos
    - sudo apt-get install libgeos-dev


[Back to top](https://github.com/emmagras/hoo-will-build-the-roads/blob/master/README.md#welcome-to-hoo)
