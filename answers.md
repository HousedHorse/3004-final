# COMP3004 Final Exam Practice Question Answers

## Multiple Choice (Concepts)

FIXME: answers up to 9 are done; need to do the rest

1. B (and probably D as well)
1. C
1. A
1. B
1. C
1. D
1. C
1. B
1. A
1. C
1. C
1. D
1. D
1. B
1. B
1. D
1. A
1. A
1. D
1. D








## Short Answer (Concepts)

### Question 1

- Functional: This category is important as it specifies *what* the application needs to be able to do from the client's point of view. It is impossible to make an application the client wants to use without knowing what they want to use it for.
- Usability: This category is an important NFR because it specifies quality constraints on the ease of use of the software. It is important to make software that is easy and effective for the client to use.
- Reliability: This category is an important NFR because the client needs to know that the application they are going to be using is robust and safe against faults and errors, both in the software and recovering from physical errors such as power failure.
- Performance: This category is important because it outlines performance-related NFRs. A user would not want to use a program that performs trivial actions in unnecessarily large amounts of time. They also wouldn't want to use an application that takes way more space on their hard drive than necessary.
- Supportability: This category is important because it specifies the limitations of the system in the context of physical hardware and the software environment the system is expected to run on. A client with a mixture of UNIX-like and DOS-based systems is not going to want to use an application that runs on windows only.
- Implementation: This category is important because it allows the designers to specify any constrains on the implementation of the system. Such constraints might include what programming language is suited to the client's needs, what types of libraries might be available to use, etc.
- Interface: This category is important because it specifies any constraints on how the application will interface with external actors such as users, external systems, etc. For example, will the application use a GUI? What APIs will it use? What API(s) will it offer, if any?
- Operation: This category is important as it specifies constraints on the operation of the system. Which users are allowed to use which parts of the application? Do users have to sign in? Are users constrained in terms of how many resources they can use at a time?
- Packaging: This requirement category is important to describe constraints on how the application is packed when it is delivered. What is included with the full system? Does it come with documentation? How is the system installed?
- Legal: This requirement is important as it specifies any legal constraints on the application. These would likely be copyright laws, privacy laws, or laws related to the client's application domain.

### Question 2

- Functional model
    - related to the functional requirements of the system
    - work products:
        - FR (and NFR) table
        - scenarios
        - scenario tables
        - actors
        - use cases diagrams
        - use case tables
- Object model
    - related to the objects in the system
    - work products:
        - initial analysis object glossary
        - class diagrams for entity, boundary, control objects
        - data dictionaries for entity, boundary, control objects
- Dynamic model
    - related to system behavior
    - work products:
        - sequence diagrams
        - activity diagrams
        - state machine diagrams

### Question 3

It would be very irresponsible for Jack to do this. Traceability is critical for having a system model that is easy to modify in the future. For example, if Jack decided to eliminate a NFR from his list of NFRs, he would need an easy way to search for that NFR everywhere else it is used in the model and modify where necessary. Without traceability, there is no easy way to do this.
Traceability also helps keep track of what requirements are being met in which parts of the system.

### Question 4

The design pattern being employed here is the proxy design pattern. The text description and the image itself are both inheriting from
some abstract image class. Each one reimplements a pure virtual member function that "displays" the image. This allows the browser to
display the proxy for the real image until it loads and leads to a better and more dynamic user experience.

TODO: paste amanda's good copy

### Question 5

The Facade design pattern is used to provide an abstraction to a more complicated interface. It allows the more complicated interface
to be more easily or more simply used either by users (external actors) or by another class within the program.

The Bridge design pattern is used to provide a series of abstractions and connect them to a series of concrete implementors.
For example, a program could have two types of views, each of which is bridged to one or more view panels depending on what type of
view it is.

### Question 6

A scenario can be thought of as an instance of a use case. It involves instantiated actors and initial analysis objects.
Scenarios should be done first as they can help establish an understanding between the client and designers and bootstrap the creation
of the actual use cases down the road (once we figure out which scenarios are good and which are garbage).

### Question 7

The includes relationship is used to abstract use cases that include redundant steps or to break down complex functionality into smaller
parts.

The extends relationship is used for exceptions; functionality that is not normal, but is instead triggered by some event within the use case. This is useful for error messages.

These are not interchangeable and most often the includes relationship should be used. Extends is only useful for error messages.

### Question 8

Shared aggregation is a weaker form of aggregation than composition. In shared aggregation, another class can
aggregate the same class that is already being aggregated and the class that is being aggregated can exist elsewhere in the program.

On the other hand, composition is a much stronger form of aggregation. If class A has a composition relationship with class B, it means
that B is a part that makes up the complete form of A. B cannot exist anywhere else in the program.

By the logic above, class A can be composed of class B and class C. But class A and class B cannot both be composed of class C.

### Question 9

State machine diagrams deal with system state at each step in the use case. Each state has one or more arrows flowing out of it
to another state(s), labeled with the condition required to take that path. State machine diagrams have a starting and an end state.

Activity diagrams deal with system activities at various stages in a use case. Each activity has one arrow flowing from/to it
and these arrows can be split by vertical bars and diamonds which represent conditionals. The activity diagrams also have a starting
and an ending point. Finally, an activity diagram can have "swim lanes" which represent the flow of control between various actors
and objects.

### Question 10

You should use an adapter pattern here. The adapter pattern will allow you to build a modern GUI front end on top of the old
`bc` program. You can make API calls to `bc` (probably via the pipe and filter architecture since `bc` is an older UNIX program)
in order to make it work with your GUI.

### Question 11

TODO: paste amanda's good copy

### Question 12

You would want to use inheritance (probably implementation inheritance) or, even more preferably, delegation to encapsulate
the shared behavior. This turns the subsystem into a high cohesion subsystem, as all the classes are related to each other
in terms of inheritance or provision/use of services.

### Question 13

Implementation inheritance is **not** a typical "is-a" relationship. It is designed to encapsulate redundant functionality and
to reuse existing code. Specification inheritance is the traditional "is-a" relationship. It describes that class B and C are
"varieties of class A".

You would want to use implementation inheritance when delegation is not an option and you have two or more classes that share redundant
functionality but are not varieties of the same thing.

You want want to use specification inheritance when you have one or more objects that are a variety of another object. This is the
traditional inheritance relationship.

### Question 14

Liskov's principle states that if some class is able to substituted for every instance of another class, the first class is a
subtype of the second. This is important as the very idea of polymorphism is the ability to substitute subclasses in place of their
parent or each other based on desired behavior.

### Question 15

- one-to-one
    - bidirectional
        - reference from source to destionation
        - reference from destination to source
    - unidirectional
        - reference from source to destination
- one-to-many
    - bidirectional
        - source has a list of destination references
        - destination has a reference to source
    - unidirectional
        - source has a list of destination references
- many-to-one
    - bidirectional
        - source has a reference to destination
        - destination has a list of references to source
    - unidirectional
        - source has a reference to destination
- many-to-many
    - bidirectional
        - source has a list of references to destination
        - destination has a list of references to source
    - unidirectional
        - source has a list of references to destination

### Question 16

- association class
    - separate class that tracks association between A and B
    - has methods to describe the relationship
    - advantage: doesn't require a unique value for each class
- qualified association
    - map
    - classes have unique values (probably a hash)
    - store the relationship in a hashmap for example
    - advantage: probably lower overhead than the association class (map lookup time is O(1))

### Question 17

- model transformation
    - changing some component of a model
    - only change one component at a time
    - change it in isolation
    - verify it after
- refactoring
    - changing some component of the source code
    - only change one component at a time
    - change it in isolation
    - verify it after

### Question 18

- forward engineering
    - writing the code
- reverse engineering
    - inferring the model from the code

### Question 19

- relational
    - advantages?
        - faster access times (in general)
    - disadvantages?
        - mapping can be non-trivial because it's a different paradigm
        - sacrifices between speed and ease of mapping
- OO
    - advantages?
        - same paradigm as OO programming
        - that means mapping is a more trivial process
    - disadvantages?
        - slower access times (in general)

### Question 20

- vertical mapping
    - table for parent and table for each child
    - inheritance mapped through foreign keys to child class table
    - parent has parent attributes, child has child attributes
- horizontal mapping
    - this can only be used if parent is abstract
    - only subclass has a table
    - each subclass table has its own copy of parent attributes

### Question 21

- blackbox?
    - tester does not know about the inner workings of the code
    - only concerns input and expected vs actual result
- whitebox?
    - tester knows about the inner workings of the code
    - test the inner workings of the component, not just input/output
- why do we need both?
    - blackbox only tells us some of the story
    - we need whitebox too

### Question 22

- we should do polymorphic testing!
    - type-cast to all three subclasses
    - test foo and bar in order
    - make a flow graph

TODO: include good copy of flow graph

### Question 23

- relates to state machine diagram
- test each transition in the diagram
    - see if we end up at expected end state each time

### Question 24

- top down
    - test top layer first
    - combine subsystems in downward fashion one stage at a time
    - this requires test stubs
- bottom up
    - test lowest layer first
    - combine subsystems in upward fashion one stage at a time
    - this requires test drivers
- sandwich
    - find target layer
    - split system into top layer, target layer, bottom layer
    - test top layer top down with target components
    - test bottom layer bottom up with target components
    - testing of top and bottom can happen concurrently
    - no drivers or stubs
    - target components not unit tested
- modified sandwich
    - find target layer
    - split system into top layer, target layer, bottom layer
    - test layers individually
        - top with stubs for tagret
        - target with drivers for top, stubs for bottom
        - bottom with drivers for target
    - combined layer tests
    - testing of top and bottom can happen concurrently
    - additional test drivers and stubs

### Question 25

- waterfall and v-model both sequential
- both involve rigorous verification, no backtracking
- v-model organized into levels of abstraction
    - arrows left to right depict flow of information between components of same abstraction level

### Question 26

- spiral and agile are both good at responding to change
    - agile is probably better at this
    - spiral is probably a little better than agile at planning, compensating for risks, costs
- agile works in sprints, iteratively
    - short delivery time
    - responds to change quickly
- spiral is also iterative, works in stages in a spiral
    - identify objectives, constraints, alternatives
    - identify and resolve risks
    - prototype and verify
    - plan next round







## Long Answer / Diagrams

### myRecipes

![fr table](figs/fr-table.png)

















## Short Answer (Ethics)

1.
