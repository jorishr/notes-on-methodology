# Test Driven Development
Testing software is similar to physical production tests:
- Unit tests: Ensure individual components work on their own. Does the heater work? Does the tank hold water?
- Integration tests: Ensure a few components work together. Does the heater heat the water in the tank?
- System (end-to-end) tests: Ensure everything works together. Does the coffee maker brew a cup of coffee?
- Acceptance tests: After being launched (sent to consumers), are they satisfied with the result? Are they confused with the button layout or breaking their coffee maker within the warranty period?

All of these tests have software analogues.

## With and without TDD
Without TDD the development process is as following:
- Choose something to work on, the specification is usually written somewhere by someone in the product team.
- Build it, following the specs.
- Test it by writing small scripts that ensure that the thing which was built does its job.

By using TDD the process you start with writing tests that *would* pass if the software was to fullfil the specifications. You than keep building until all the tests can be passed. The main advantage is that the *specification have to clarified* when the test are being written. 