# COMP3004 Final Exam Notes

## Software engineering

### What is it?

- requirements analysis
- building a software system to accomplish a task
    - a software system is big and complex
    - not just a dinky little program
- reliable, modifiable process

### Why is it necessary?

- huge systems and projects difficult to manage
- we need a plan
- reliability, modifiability






## Build models

- functional model

- dynamic model

- object model

### Why do we need them?

- get an idea of full system
- requirements
- clarify details
- make sure client and design team on the same page

### What are they?

- functional model
    - FR, NFR (table, FURPS+)
    - use cases (diagrams, tables)
        - high level (don't forget the box!)
        - detailed (includes and extends)
- dynamic model
    - state machine diagrams(s)
    - activity diagram(s)
    - sequence diagram(s)
- object model
    - class diagram(s)
    - data dictionaries

### Traceability -- what and why?

- number entries in tables for traceability
    - esp. FR/NFR and data dictionary
- helps with maintenance of design








## Software development life cycle

### Phases and work products of each

1. Requirements Elicitation
    - work products? the functional model!
        - FURPS+ table
        - use case diagram
        - scenarios, use cases
1. Analysis
    - work products? the object and dynamic models!
        - class diagrams
        - activity / sequence / state machine diagrams
1. High Level System Design
    - work products?
        - system architecture
        - subsystem decomposition
1. Detailed Object Design
    - FIXME: add work products
1. Implementation
    - FIXME: add work products
1. Testing
    - FIXME: add work products
1. Deployment / Maintenance
    - FIXME: add work products

- where does the client's knowledge end and begin again?
    - ends right after analysis
    - starts up again half way through testing (once we start testing final system)

### Requirements elicitation

#### FURPS+ Tables

- FURPS+
    - F: functional
        - if you can make a use case for it, it's functional
        - and vice versa
        - "what can the actors do with the system?"
    - U: usability
        - ease of use requirements
    - R: reliability
        - recover from error
        - stability
        - security
    - P: performance
        - performance metrics
        - task X should be complete within Y seconds on a dataset of size Z
    - S: supportability
        - future maintainability
        - what kinds of platforms/hardware can the system run on?
    - +: Implementation
        - implementation-specific requirements
    - +: Interface
        - how system interacts with actors (GUI, CLI, etc) -- boundary object requirements
        - how it interacts with external systems
    - +: Operation
        - which users are allowed to do what
    - +: Packaging
    - +: Legal
- FURPS+ should be measurable, **reasonable**, specific -- don't state the obvious
    - not as simple as "the system should be easy to use"

#### Use Case Diagrams

![overview of UC diagrams](figs/uc-dia-overview.png)

#### Use Case Tables

- FIXME: fill me out

### Analysis

- TODO: work on me!!

### High-level system design

- TODO: work on me!!

### Detailed object design

- TODO: work on me!!

### Implementation

- TODO: work on me!!

### Testing

- TODO: work on me!!

### Deployment and maintenance

- TODO: work on me!!









## Models in requirements analysis

### Object model

- TODO: work on me!!

### Dynamic model

- TODO: work on me!!

### Functional model

- TODO: work on me!!











## Requirements elicitation

### Why do it?

- TODO: work on me!!

### FR and NFR (FURPS+)

- TODO: work on me!!

### Scenarios and use cases

- TODO: work on me!!

### UML use case diagrams

- TODO: work on me!!

### Use case tables

- TODO: work on me!!








## Analysis

### Object model

- TODO: work on me!!

### Dynamic model

- TODO: work on me!!








## High level design

### Design goals

- TODO: work on me!!

### Subsystem decomposition

- TODO: work on me!!

### System design strategies

- TODO: work on me!!







## Detailed object design

### Types of inheritance

- TODO: work on me!!

### Liskov's principle

- TODO: work on me!!

### Contracts

- TODO: work on me!!







## Implementation

### Mapping objects to collections

- TODO: work on me!!

### Model transformations

- TODO: work on me!!

### Mapping associations to collections

- TODO: work on me!!

### Mapping associations to storage

- TODO: work on me!!

### Buried associations

- TODO: work on me!!

### Association tables

- TODO: work on me!!

### Vertical/horizontal mapping of inheritance to storage

- TODO: work on me!!







## Testing

### Blackbox vs whitebox

- TODO: work on me!!

### Unit testing (path, equivalence, boundary, state, polymorphism)

- TODO: work on me!!

### Integration testing (top-down, bottom-up, sandwich, modified sandwich, test stubs, test drivers)

- TODO: work on me!!

### System testing (functional, performance)

- TODO: work on me!!






## Software development life cycle model

- Software Development Life Cycle Process:
    - An approach to performing system development activities.
    - Goals and activities will remain the same between each different process
    - But the order and focus of each activity will be different.

- Two Main Types:
    - Activity-Focused Processes
        focus is on **development activities**.
    - Entity-Focused Processes
        focus is on the **products** that are created.

### Agile

- TODO: work on me!!

### Waterfall

- Activity Based Development Process
- Each activity is done in sequential order
    - Goal: Never repeat an activity once completed.
    - Strategy: Constant Verification at each step.

- TODO: add diagram.


### V-model

- Characteristics
    - Activity Centred


### Spiral

- TODO: work on me!!








## Ethics

### Professionalism

- TODO: work on me!!

### Code of ethics

- TODO: work on me!!

### Process for making ethical decisions

- TODO: work on me!!
