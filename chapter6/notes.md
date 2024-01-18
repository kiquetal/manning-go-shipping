### Testing framework, mocking and dependency injection

- Always start with an interface
- Use a mocking framework to mock the interface
- Use dependency injection to inject the mock into the code under test


### Testing framework

- Stub are very simple implemention of any structures. They are used to return a value or throw an exception when a method is called.
- Stub can be great placeholder while code is under development.
- Mocks are stubs with an expectation. They are used to verify that a method is called with the right parameters.

### Types of Test

| Type | Pros | Cons |
| ---- | ---- | ---- |
| Stub | Easy to create and manipulate | Verification can become complicated|
| Mock | Records interactions for later verification | More complex setup and teardown | 
| Fake | Higher-fidelity interactions with a simulated system | Complicated to write and maintan | 
