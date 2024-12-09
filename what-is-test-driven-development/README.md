<h1>
  <span class="headline">Java Test-Driven Development</span>
  <span class="subhead">What is Test-Driven Development?</span>
</h1>

**Learning objective:** By the end of this lesson, students will be able to examine the three-phase cycle of test-driven development (TDD) and how TDD supports Agile development processes.

### What is test-driven development (TDD)?

Test-driven development follows a three-phase process:

1. **Red**: write a failing test (including possible compilation failures). We run the test suite to verify the failing tests.
2. **Green**: write just enough production code to make the test green. We run the test suite to verify this.
3. **Refactor (blue)**: remove any code smells. These may be due to duplication, hardcoded values, or improper use of language idioms. If we break any tests during refactoring, we prioritize getting them back to green before exiting this phase.

![Red, green, refactor](./assets/1-rgf.png)

The three phases of this cycle are the essential building blocks of test-driven development.

Note: TDD is a perfect match for the ideals and principles of the agile development process, with a great striving to deliver incremental updates to a product with true quality, as opposed to quantity. The confidence in your individual units of code that unit testing provides means that you meet this requirement to deliver quality, while eradicating issues in your production environments.

### Agile development with test-driven development

TDD comes into its own when **pair programming**, however. The ability to mix up your development workflow, when working as a pair as you see fit, is nice. For example, one person can write the unit test, see it pass, and then allow the other developer to write the code to make the test pass.
