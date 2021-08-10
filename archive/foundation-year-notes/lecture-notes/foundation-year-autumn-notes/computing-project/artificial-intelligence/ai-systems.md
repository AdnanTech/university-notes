# AI Systems

## System View

A systems view is the way in which a complex society can function. It's a more Hard AI approach. The idea of the complex society with humans as the organisational unit, can be extrapolated into complex computers, where programs are the organisational unit. It is also the way the biological system is built. There are 2 main design philosophies when it comes to system views:

1. One large system \(One large program\)
2. Lots of smaller tasks \(small programs\) that interact with each other to essentially make one system

Method 2 is a lot more useful in terms of task decomposition. As the smaller tasks will interact with each other, so they can be tested using modular methods. As well as each task only needs to know about it's own I/O and access certain data, this can be seperate from it's surrounding tasks. **Each task serves a specific purpose**. There is more possibility with this method, as we can have hierarchical tasks.

### Biological System

The biological system can be seen as a hierarchy: Atoms and molecules go to cells which go to tissue which go to orgrans, which in turn make an organ system. The organ system is at the top of the heap, it can use all subsumes underneath it

So, the brain/nervous system can be abstracted into a system based view. Where the brain is essentially a neural processing system, and the processes \(functions\) can be divided into:

* Higher functions
  * A good example of a higher function would be recognition, where the function requires different brain centeres exchanging information. The combination of these signals and their interpretation is the subject of learning. This is the upper part of the brain, the pink tissue. This hold stuff we learn, the crystalised intelligence.
* Autonomic functions
  * These include functions such as reflex actions. They are not learned, they just happen. For example, we do not need to remind ourselves how to breathe. This is the brain stem, the lower part of the 2 sectors of the brain. This stuff is pre programmed at birth, we do not need to learn how to do these functions. This section executes a lot faster than high functions.

There is an argument that pain is essential to learning, to protect our biological systems, this becomes apparent in trauma patients.

### Life System

In life, there is no single program, but a subset of smaller systems interacting each other to make it look like there is one program. Some are simple systems, such as retracting the hand from a hot surface \(the temperature sensor is closely coupled to the tendon actuator\). This suggests that an artificial life form should adopt a similar approach, being that of smaller systems that interact with each other.

This can be seen in abstraction with how we walk. Does the brain need to control the ankle joint directly? It could, but it’s not the easiest way of organising things. The ankle joint is a small system that can cater for itself, it allows for us to land our foot flat on the floor, its like controlled falling. The leg is a system that relies on the ankle joint. And so on. The brain only decides that we want to walk, everything else works for itself.

## Subsumption

Paper by MIT researcher Rodney Brook written in 1986 introduced subsumption architecture, to help build AI using a systems view \(so a system comprised of smaller systems\). Subsumption architecture has its origins in the analysis of societal and biological systems

Basic idea: Uses human biology theory and couples “sensory information”, at the bottom of the heap, to “action selection", at the top of the heap, in a bottom up manner. Does this by decomposing some behaviour into a set of sub-behaviours. Each layer achieves a level of competence \(where competence mean good at something\). Higher levels can utilise of “subsume” \(use\) these lower level to create viable behaviours.

### Visualised

A robot that explores the world:

![](../../../../../../.gitbook/assets/image%20%2846%29.png)

* So “avoid objects” is the lowest level. It’s simple and easy to achieve, and is sensory motion
* “Wander around” is a behaviour but it’s going to require “avoid objects” to do it successfully, is action motion
* “Explore world” is a higher level idea
* The outputs from “explore world” can influence “wander around”
* The outputs from “wander around” can influence “avoid objects”
* But only “avoid objects” actually drives the wheels or legs

### Assumptions

Subsumption makes some assumptions, these are:

* Brooks is concerned with robots that exist in some environment.
* And interact with it.
* Gives rise to the notion of embodiment \(things inside the robot\).
* Also the notion of perception and action.
* The solution is a distributed processing system.

Walking is high level, joints are lower level. 

## Sources

* [Brook's Paper](https://people.csail.mit.edu/brooks/papers/AIM-864.pdf)









