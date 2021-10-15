---
description: 15/10/2021
---

# Arrays & For Loops

## Key Concepts

* Abstraction
* Modularization
* Classes as types
* Class diagram
* Object diagram 

## Example - A digital clock 

### Modularization

This is the process of dividing a whole into multiple well-defined parts which can be built and examined separately and which interact in well defined ways. 

### Abstraction

This is the ability to remove unnecessary details from a problem to focus attention on a higher level of a problem.

### Modularization of a digital clock 

Is a digital clock made up of a 4 digit display or 2 2 digit displays?

### Abstraction of number displays

* 2 displays
  * minutes 0 - 59, rolls around to zero after 59 
  * hours 0 - 23, rolls around to zero after 23
* Noticing common behaviour gives rise to abstraction. 
  * A `NumberDisplay` object has a current value in range 0 - (limit - 1)
