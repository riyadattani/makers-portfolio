# I can TDD anything

###### Reflect: What does it mean to be able to TDD anything?

- To understand and follow the Red - Green - Refactor cycle.
  - Red: write a failing test
  - Green: write the simplest code to pass the test
  - Refactor the code to be clean and follow good convention without adding any additional functionality
- To preferably write a feature test which tests how a feature would work from the users perspective and then write (multiple) unit tests to pass the feature test. This is ideal for bigger projects as it breaks down the program into smaller steps.
- To use dependency injection, doubling and mocking in unit tests to remove dependencies of classes when testing.
- To design tests that drive you to a solution.
- To aim to test the behaviour of a class rather than the state of them.
- To be wary of edge cases and writing tests for them too.

###### Plan: List evidence you aim to collect that would together show you have credibly achieved this goal

- An example showing the use of dependency injection/ mocking/ doubling/ stubbing to show isolation of tests.
- An example of test-driving a project without using a testing framework.
- An example of TDD in an unfamiliar language.
- An example of TDD using a feature test which is passed through smaller unit tests.

**Q: Can you TDD confidently? YES **

###### Reflect: How does each of the following examples of your best work show evidence of achieving this goal? (e.g. Diode projects, Github repos)

- [Bank Tech Test](https://github.com/riyadattani/bankTechTest/blob/master/spec/statementSpec.js )
  - Example of mocking out the account class which is needed to create a statement.
  - Checked if this mock works by commenting out the account class and confirming that the tests for the statement class pass.
- [Airport challenge](https://github.com/riyadattani/airport_challenge/blob/master/spec/airport_spec.rb)
  - Stubbing weather class for randomness: since the weather is randomly generated, I stubbed this in the specs for the airport class.
  - Doubles: doubles of the weather class and the plane class were used to keep the classes independant when testing.
- Note app in JS
  - Test driving by creating my own [testing framework](https://github.com/riyadattani/single-page-notes-app/blob/master/tests/assert.js)
  - Used [dependency injection](https://github.com/riyadattani/single-page-notes-app/blob/master/src/note-controller.js) in the ‘renderHtml’ function so that ‘element’ could be mocked out in the tests
- [Thermostat](https://github.com/riyadattani/thermostat_JS/commits/master)
  - TDD in thermostat in an unfamiliar language: javascript.
  - The commit history shows how this task was broken down into smaller features and each was implemented using the TDD process.
- [RPS challenge](https://github.com/riyadattani/rps-challenge)
  - Test driven using a feature test to begin with and then smaller unit tests to pass the feature test.

###### What feedback have you had?

_Steven during a process workshop_, “You have a good TDD process. You started off with the easiest test and passed it in the most simplest way. Once you started developing the program, you changed your method appropriately. You followed the RED-GREEN-REFACTOR method very well.”

_Sophie (Coach) during observation_, “You have a good process: you drew a plan/model that seemed good enough to start with, you wrote a simple test and proved you were following TDD. I would ask more questions on how the command line app would work and avoid using puts and gets as it constricts your app from growing.”
