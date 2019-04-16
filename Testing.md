## Testing
  - Input to testing
    - functional model
    - non-functional requirements
    - subsystem decomposition
    - source code
  - Output from testing
    - deliverable system
![test Chart](figs/testingwp.png)
  - What is testing?
    - the process of finding differences between:
      - specified system behaviour
      - observed system behaviour
    - systematic attempt to find faults in a planned manner
  - Purpose
    - break the system
    - testing is based on the falsification of system models
  - How do we test software?
    - design tests that expose the defects in the system
  - Who does the testing?
    - developers not involved in design or implementation
    - specialized testers
  Terminology
    - failure:
      - deviation of observed behaviour from specified behaviour
    - error state:
      - system is in a state where further processing will lead to failure
    - fault:
      - a defect or bug
      - the mechanical or algorithmic cause of an error

### Testing Basic Concepts

#### Software reliability
  - degree to which observed behaviour conforms to specification
  - Techniques for increasing reliability
    - fault avoidance
      - detect faults statically, without model execution
      - prevent faults before system is released
      - includes:
        - use of development methodologies
        - configuration management
        - verification
    - fault detection
      - identify error states and faults before release
      - includes
        - debugging (uncontrolled)
        - testing (controlled)
    - fault tolerance
      - cope with faults and system failures
      - recover from faults and failures at runtime
        - for example, using redundant components
        
#### Code reviews
  - manual inspection of parts of the system without execution
  - performed by review team
  - Two types of review
    - walkthrough
      - developer presents the code
    - inspection
      - review team checks everything
  - Goal of code reviews
    - check code against requirements
      - both functional and non-functional
    - check for algorithm efficiency
    - check accuracy and completeness of comments
    
#### Testing approach
  Main things to check
  - wide range of inputs
  - invalid inputs (e.g. outside range, zeros, wrong data type)
  - boundary cases
  - test planning
  - usability testing
  - unit testing
  - integration testing
  - system testing
    - functional testing
    - performance testing
    - acceptance testing
    
#### Blackbox and whitebox testing
  - Blackbox
    - test cases are not based on the code’s internal structure
    - focus is on input/output behaviour of test component
    - ignores internal aspects of component
  - Whitebox
    - test cases are based on the code’s internal structure
    - focus is on internal structure of the test component
    - ensures that everything is tested:
      - every state in the dynamic model
      - all object interactions
  - Unit testing must include both blackbox and whitebox
  
#### Faults, error states, failures
  - Fault
    - Types of faults
      - algorithmic
        - may be introduced during implementation, design, or analysis
        - examples:
          - data structure overload
          - lack of initialization
          - performance problems
      - mechanical
        - occur even if implementation is correct
        - examples:
          - fault in the programming environment
          - power failure
![fault](figs/fault.png)
  - State
    - An error state would be a train running on the track reaching that fault 
#### Test cases
  - set of inputs and expected results that exercise a component
  - goal is to cause failures and detect faults
  - Every test case has these attributes:
    - unique name
      - should be derived from associated requirement or component
    - component under test
      - operations, classes, subsystems being tested
    - input
      - set of input data or commands entered by actor (tester or test driver)
    - expected output
      - expected results against which output of test is compared
  - Test case development dependencies
    - functional testing
      - depends on functional model (use cases)
    - unit testing
      - depends on definition of subsystem interfaces
  - Test cases can be related by associations
    - aggregation
      - test case can be decomposed into a set of sub-tests
    - precedence
      - used to specify when one test case must precede another
![testcases](figs/testcases.png)

#### Test stubs and drivers
  - Issue:
    - we need to test isolated components
      - some code has to call the test component
      - some code has to execute when the test component calls other code
    - we need to substitute the missing parts
  - Solution:
    - write test drivers to call the test component
    - write test stubs to simulate the called portions of code
  - Test driver
    - simulates part of the system that calls the test component
    - passes in the test inputs
    - displays the results of the test
  - Test stub
    - simulates the component that is called by the test component
    - provides the same API as the simulated component
    - must return expected value
    - must simulate exact behaviour or may cause test case failure
    - may be more efficient to use than actual called component
    
#### Corrections
  - a change to a component in order to repair a fault
  - can introduce new faults
  - Managing corrections
    - problem tracking
      - documentation of errors and code fixes
    - regression testing
      - re-execution of all prior tests after a code fix
      - ensures that all previously working functionality is intact
      - this should be as automated as possible
    - rationale maintenance
      - documentation of reasons for change
      - ensures that no new faults are introduced by violating previous assumptions
### Usability Testing
  - finding differences between system and user expectations
  - Possible problems
    - UI details
    - layout of screens
    - sequence of interactions
    - hardware
  - Possible approaches
    - developers set out test objectives
    - participants accomplish predefined tasks
    - developers observe and collect user performance data
  - Three types of usability tests
    - scenario test
      - users presented with scenario of system
      - developers gauge user reactions to how scenario models work tasks
      - can be achieved with story boards or prototypes
    - prototype test
      - users presented with software that implements key aspects of system
      - vertical prototype: one use case is completely implemented
      - horizontal prototype: a single layer is implemented
        - for example: UI prototype
    - product test
      - users presented with functional system
