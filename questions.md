# COMP3004 Final Exam Practice Questions

## Multiple Choice (Concepts)

1. Why is software engineering necessary?
    - A) It's fun
    - B) Huge systems and projects are difficult to manage
    - C) It isn't necessary
    - D) It's an easy way for people to work together
1. What is not a build model?
    - A) Functional model
    - B) Dynamic model
    - C) Static model
    - D) Object model
1. What is not an example of a dynamic model?
    - A) Use case diagrams
    - B) State machine diagrams
    - C) Activity diagrams
    - D) Sequence diagrams
1. Why is traceability important?
    - A) It's easy to trace back the design of the code
    - B) It helps with maintenance of design
    - C) It helps the developer keep on track
    - D) It helps with the users to keep on track
1. Where does the client's knowledge end?
    - A) It ends after implementation
    - B) It ends after testing
    - C) It ends after analysis
    - D) It ends after requirement and elicitation
1. What is not a original design pattern?
    - A) Creational
    - B) Structural
    - C) Behavioral
    - D) Architectural
1. What is not part of the behavioral design patterns
    - A) Command
    - B) Strategy
    - C) Facade
    - D) Observer
1. What is not a design goal?
    - A) Performance
    - B) Supportability
    - C) Cost
    - D) Maintenance
1. What are the functions of the ball and socket in a component diagram?
    - A) The ball provides the service and the socket uses the service
    - B) The ball uses the service and the socket provides the service
    - C) The ball stores the service and the socket initializes the service
    - D) The ball provides the service and the socket initializes the service
1. Which of the following is not an architecture style?
    - A) 4 tier
    - B) peer-to-peer
    - C) client-to-peer
    - D) pipe and filter
1. Contract does not include which of the following constraint
    - A) precondition
    - B) invariant
    - C) variant
    - D) postcondition
1. What are some advantages to use design pattern?
    - A) Encapsulating data stores
    - B) Maintainability
    - C) Maintaining consistency
    - D) A and C
1. Which is not part of transformation?
    - A) Model
    - B) Reverse engineering
    - C) Forward engineering
    - D) Database
1. Which best describes Horizontal mapping
    - A) superclass and subclass each have their own table
    - B) only the subclass has a table
    - C) access to one object involves multiple table retrievals
    - D) A and C
1. Which statement is true?
    - A) Horizontal mapping facilitates modifiability
    - B) Vertical mapping takes more time to retrieve data
    - C) Horizontal mapping schemas are simpler than vertical mapping schemas
    - D) Both A and B
1. Which is not part of the Relational database?
    - A) schema
    - B) primary key
    - C) unique key
    - D) private key
1. Which best describes blackbox testing?
    - A) Tester is unaware of internal system
    - B) Tester is aware of internal system
    - C) Easier to test than whitebox testing
    - D) Both A and C
1. Which is not part of integration testing?
    - A) Hamburger
    - B) Modified Sandwich
    - C) Test Stubs
    - D) Bottom-Up
1. Which best describes waterfall life cycle?
    - A) Sequential
    - B) Iterative
    - C) Never revisit an activity once completed
    - D) Both A and C
1. Which is not a possible course of action?
    - A) I win, you lose
    - B) I lose, you win
    - C) We both win
    - D) We both lose
1. Verification and configuration management happens in
    - a) Fault avoidance
    - b) Fault detection
    - c) Fault tolerance
1. Testing and debugging happens in
    - a) Fault avoidance
    - b) Fault detection
    - c) Fault tolerance
1. Recovering from faults and failures in terms happens in :
    - a) Fault avoidance
    - b) Fault detection
    - c) Fault tolerance
1. All of these are types of System Testings except:
    - a) Functional testing
    - b) Usability Testing
    - c) Performance Testing
    - d) Acceptance Testing
1. One of these testings is mainly performed by the client:
    - a) Functional testing
    - b) Usability Testing
    - c) Performance Testing
    - d) Acceptance Testing
1. \_\_\_\_\_\_\_ simulates the called portion of the code:
    - a) Test drivers
    - b) Test stubs
    - c) Unit Testing
1. \_\_\_\_\_\_\_\_ testing requires no test stubs:
    - a) Big bang Testing
    - b) Path Testing
    - c) Bottom-Up Testing
    - d) Polymorphism Testing
1. \_\_\_\_\_\_\_\_ testing requires no test drivers but MANY test stubs:
    - a) Big bang Testing
    - b) Path Testing
    - c) Top-down Testing
    - d) Polymorphism Testing
1. Which system Testing has most of its cases derived from functional requirements?
    - a) Field Testing
    - b) Functional Testing
    - c) Acceptance Testing
1. System is deemed validated when :
    - a) functional and acceptance testing has no failures
    - b) functional and path testing has no failures
    - c) functional and performance testing has no failures
1. Containers are type of :
    - a) implementation inheritance
    - b) specification inheritance
    - c) delegation
1. Two types of contracts associated with an operation:
    - a) post condition and pre condition
    - b) pre condition and invariant
    - c) invariant and post condition
1. Example of optimizing object model for expensive results like frequently called operations :
    - a) caching
    - b) forward engineering
    - c) reverse engineering
1. \_\_\_\_\_\_\_ is a solution for optimizing "many" side associations :
    - a) contracts
    - b) qualified associations
1. \_\_\_\_\_\_ is a meta model for data:
    - a) schema
    - b) primary key
    - c) foreign key

## Short Answer (Concepts)

1. Describe each of the FURPS+ requirement categories and why each one is important to the requirements elicitation process.
1. Give an overview of the three models of the requirements elicitation/analysis process and list the work products encompassed by each (diagrams and tables).
1. Jack wants to save on printer ink and skip writing numbers for the functional and non-functional requirements in his document. Explain to Jack why this is probably not a smart idea.
1. A browser displays alternate text before an image finished loading. What design pattern is being employed here? Draw a small class diagram to demonstrate.
1. Karen is confused about the difference between the "Facade" and "Bridge" design patterns. Explain the difference to Karen.
1. What is the difference between a scenario and use case? During the requirements elicitation process, which of the two would you try to come up with first and why?
1. Explain the difference between the "includes" relationship and the "extends" relationship in UML use case diagrams. Are the two interchangeable? Why or why not?
1. What is primary difference between composition and shared aggregation? Would it be possible for two classes to be composed of the same object? Would it be possible for one class to be composed of two or more objects? Why or why not?
1. State machine diagrams and activity diagrams may appear similar at first glance. What is the primary difference between the two?
1. You want to modernize the old UNIX `bc` program to turn it into a GUI calculator. Assume that it would be more efficient to use the old `bc` code than to rewrite the calculator logic from scratch. What kind of design pattern might be beneficial here and why?
1. Draw a UML state machine diagram for an application that allows you to write test questions and add them to a remote test bank.
1. Suppose you have a subsystem with three classes that all share similar functionality. Unfortunately, this subsystem has very low cohesion, as none of the classes use each other's services. What transformation might you apply to your model to fix this problem?
1. What is the difference between implementation and specification inheritance? Give an example of when you might use each?
1. Why is Liskov's principle important for polymorphism as we know it?
1. Suppose you have two classes (A and B). What are the four types of possible associations between A and B and how would you map each one to source code from a UML class diagram?
1. What are the two ways of optimizing associations between classes? List the advantages and/or disadvantages of each in as much detail as possible.
1. Explain the difference between model transformation and refactoring using an example.
1. Explain the difference between reverse engineering and forward engineering using an example.
1. Consider relational databases and OO databases. List one advantage and one disadvantage of each in the context of implementing a C++ program that needs to interface with a database.
1. What is the difference between vertical and horizontal mapping in the context of mapping inheritance relationships to storage? Explain the trade-off between the two.
1. What is the difference between blackbox and whitebox testing? Why is it important to use both of them when unit testing?
1. You have a class A which is subclassed by classes A1, A2, and A3. A has virtual methods foo() and bar(). What kind of testing should you do to ensure that A1, A2, and A3 are all behaving properly?
1. Explain the process of state-based testing as it relates to a specific type of UML diagram. (Hint: What UML diagram deals with state?)
1. Name the four types of integration testing and describe each one. You may wish to support your explanation with an example.
1. Compare and contrast the waterfall and v-model life cycle models.
1. Compare and contrast the spiral and agile life cycle models.








## Long Answer / Diagrams

This section contains a few system descriptions. For each description, do the following:

1. Create a FURPS+ requirements table and elicit at least 2 requirements from each category.
1. Draw a high level use case diagram. Include several high level use cases, the system boundary box, all applicable actors.
1. Draw one or more detailed use case diagrams. Include all relevant actors and use cases, and use both includes and extends relationships.
1. Draw a state machine diagram for **ONE** use case.
1. Draw a sequence diagram for **ONE** use case.
1. Draw an activity diagram **ONE** use case.
1. Choose the best architecture for the system. Indicate which architecture you are using, and describe whether it will be an open or closed architecture.
1. Create a reasonable subsystem decomposition for the system.
1. Explain a few design patterns you could use in your system.

---

Consider the myRecipes system. The system allows users to access recipes on their own local host and access recipes on peer hosts that are part of the system. The system supports three kinds of users: cooks, chefs, and assistant chefs.

Assistant Chefs can do the following:

- browse recipes stored locally
- create new recipes locally
- edit recipes stored locally

Chefs can do the following:

- everything assistant chefs can do
- browse recipes on other peer hosts
- download recipes from other hosts

Cooks can do the following:

- browse recipes on other peer hosts









## Short Answer (Ethics)

1. Suppose you are developing an application to help users do their taxes. In order to help generate a revenue stream, your boss demands that you include a crypto miner inside the application that can run undetected and mine bitcoin for the organization. Use the ethical decision making process to determine the best course of action.
