# ![[tktk Module Name] - tktk Microlesson Name](./assets/levels-of-testing.png)

**Learning objective:** By the end of this lesson, students will be able to examine the Test-Driven Development frameework and how it is used in the application of unit, integration, and acceptance testing. 

### Levels of Testing

As you start practicing TDD, you will write different levels of tests. Your application should be composed of tests in
each of the following levels. Each of these levels focuses on a different aspect of code and provides different
feedback. Let's look at them one by one.

- **Unit testing** : Here you est individual software components to verify if the individual unit does the right
  thing in isolation.

- **Integration testing**: Here you test multiple units together to verify if they work correctly as a unit.

- **Acceptance testing**: Here you test the full system to verify if it works as per user expectations. It is often
  referred to as functional testing.

![img.png](lecture/images/2-test-pyramid.png)

The point image above is to convey that you should have many more unit tests than functional or integration tests.

### Benefits of unit testing

As discussed previously, unit testing is no longer a post-development exercise. It is as equally important as writing
production code and must be done up front. It enhances team productivity by providing solid foundations. Let's look at
the benefits unit testing offers in detail.

**Determines Specifications**

Before we start the journey of coding a component we must try to determine what the component must do? Try to build a
test case of the possible inputs and the possible outputs. The act of building test cases at the start helps to clarify
the expected behavior of the component.

If we are unable to come up with a test, it means that the specifications are not explicit enough and require more
thinking.

**Provides Early Error Detection**

Unit tests are proof of working code. They are executed in every build and can detect failures at the first instance.

Unit tests can detect not only coding bugs but flaws in product specifications as well. A unit test demonstrates
progress; thus, as soon as a component is complete, it can be demo-ed to the stakeholders to find gaps, if any. The
sooner a bug is uncovered, the cheaper it is to fix.

**Supports Maintenance**

Product specifications evolve over time. These changes lead to development cycles. In each of these cycles, the team has
to understand how the existing code works before team members can make any changes. Unit tests help in understanding the
intended behavior without being bogged down by the actual code. A well-written unit test suite serves as a productivity
boost for the team.

**Improves Design**

Unit tests are the first client of the code being tested. They uncover various issues that a client can face while
interfacing with the code being tested. Unit tests make us think in terms of the expected input and the expected output.
For internal components (service, utilities, etc.), this can help in classifying responsibility boundaries. It helps in
improving product specifications by exposing gaps in the interface design.

**Product Documentation**

Unit tests describe how a piece of code works—that is, the expected output for a given input. They always describe the
latest state of a specification, as they are kept in sync with the code changes.