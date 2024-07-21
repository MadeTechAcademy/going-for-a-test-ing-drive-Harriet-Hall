[![Review Assignment Due Date](https://classroom.github.com/assets/deadline-readme-button-22041afd0340ce965d47ae6ef1cefeee28c7c493a6346c4f15d667ab976d596c.svg)](https://classroom.github.com/a/ycVsfoVh)
# test-ing--drive

In bootcamp you explored the principles of TDD (what is a test, writing a test before code, red-green-refactor, etc.). Before we meet up again to go deeper into testing, I'd like you to explore how testing works on your projects.

To submit your answers, you must first create a branch of this repository, then edit this README file.

1. Describe the approach to TDD on your delivery. In general, how strict are people writing tests before code? (This is not a judgement, just an observation of what you are noticing). What makes it difficult to start with tests? What might make it easier?

Due to the nature of the project, not very strict. Old Bichard, originally written in Java with minimal documentation, is now being rewritten in Typescript and then tested. Development is not being led by tests as it is unclear what the legacy code actually does or is meant to do. It seems like, while desirable, TDD is not always the best approach depending on the project. TDD has been implemented in parts of the front-end code,although I have not seen this myself. In some ways, testing a function that has already been written is easier as it is evident how it is expected to behave, however, I found that my lack of domain knowledge means that I am testing code I 'haven't written myself. This can be very challenging when understanding function/variable names and syntax I am not familiar with.


2. What testing frameworks are in use? Is the same framework used for everything, or do you have a framework for testing code, and one for testing a website or service?
Cucumber testing framework with test written in Gherkin - Behaviour Driven Development - e2e tests 
Cypress testing framework - e2e and component tests 
CircleCi - runs all tests - back-end + front-end before pull requests are merged
Jest - unit tests for front end functions 
Comparison tests - specific to Bichard - comparing old Bichard + new Bicard output the same thing 

3. Looking at the language(s) used, list at least 5 other testing frameworks. What do they have in common, and what's their unique proposition?
Vitest - has all the features of Jest but better suited for good for modern projects  
Storybook - focuses on UI components in isolation
Mocha - robust and allows users to work with external library eg.Chai & supports async testing
Puppeteer - mainly used for browser automation and integration testing
Playwright - like Puppeteer but supports multiple browsers 
They all support Typescript 

4. Using a coverage tool, what is the test coverage on the project (If there's more than one project, choose one). What might that result suggest? In what area would you discuss adding more tests?
High coverage
It's a complex project with many moving parts that are dependent on each other. It is important for developers on the project that everything is tested well. Insufficient testing could lead to unwanted behaviours - as the project deals with sensitive data, this could have negative repercussions on members of the public

5. Looking at the tests written, how confident would you say they:
    - describe what is happening 
Very confident

    - correctly document what the code should be doing
Very confident

    - drive development of the code (because of this test this feature *and only this feature* was made)
Not confident as they are written after the feature has been created 

