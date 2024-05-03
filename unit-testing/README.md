# ![[tktk Module Name] - tktk Microlesson Name](./assets/unit-testing.png)

**Learning objective:** By the end of this lesson, students will be able to understand unit tests and how to implement these principles. 

### Characteristics of Good unit tests

Tests should be written with the same focus and clarity as the production code. We must refactor test cases so that `
they are kept lean and correct. Tests will only reap benefits if people can understand and rely on them.

- **Readable**: One of the goals of a test is to educate its reader about what the unit being tested will do. If the
  tests are not readable then the reader will not be able to understand when the tests will fail. A good unit test
  case has a meaningful name so that the reader understands the behavior of unit being tested without looking
  at implementation details.

- **Fast**: Tests should run in few seconds so that they provide quick feedback. If tests take more time, the programmer
  will look for ways to skip the tests. Unit tests must mock external dependencies so that the tests run fast and
  independent of external services. Mocking allows testing of a unit of code by simulating behaviour of its dependencies
  in a controlled manner.

- **Independent and Isolated**: Good unit tests are independent of execution order. They don't rely on other unit tests
  for them to work correctly. They should run independently in their own isolated environment.

- **Correct**: A good unit test does what it says. A test case should correspond to a single case (i.e., behavior).
  Often tests don't do what their name suggests. This is very risky, as in that case you can't trust your
  tests.

- **Environment agnostic**: A litmus test for any software project is the following: "_Can you check out the code
  on a clean developer machine and run the full build including tests without any problem._" Most of the time, we find
  that unit tests fail because they depend on some external factor. The external factor could be a file at a particular
  location, an environment variable, or something else. This leads to brittle tests. A good unit test does not depend on
  the environment.

- **Repeatable**: A good unit test produces the same result each time you run it. Test execution should be automated
  using the build tool. They should be part of the automated build process so that they run each time you execute build.
  When tests start failing randomly, programmers start ignoring them. These random test failures are difficult to
  reproduce and normally happen on external systems like continuous integration servers. Team should ensure
  that failing tests are fixed as soon as they are discovered.

### Syntax for Unit Testing

There is a list of assert statements available on [this page](https://www.baeldung.com/junit-assertions) that you can
use as per your requirements. Below is a list of some of the most common assert statements.

| Method                                                | Checks for                                                                                  |
|-------------------------------------------------------|---------------------------------------------------------------------------------------------|
| `void assertEquals(boolean expected, boolean actual)` | Checks that two primitives/objects are equal                                                |
| `void assertTrue(boolean condition)`                  | Checks that a condition is true                                                             |
| `void assertFalse(boolean condition)`                 | Checks that a condition is false                                                            |
| `void assertNotNull(Object object)`                   | Checks that an object isn't null                                                            | 
| `void assertNull(Object object) `                     | Checks that an object is null                                                               | 
| `void assertSame(object1, object2)`                   | The `assertSame()` method tests if two object references point to the same object           |
| `void assertNotSame(object1, object2)`                | The `assertNotSame()` method tests if two object references do not point to the same object |
| `void assertArrayEquals(expectedArray, resultArray)`  | The `assertArrayEquals()` method will test whether two arrays are equal to each other       |