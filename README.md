# Java Service Testing and Software Quality

A Java coursework project implementing **appointment, contact, and task management services**, with unit tests focused on validating inputs and checking service behavior.

## What is in this repository?

| Component | Implementation | Unit tests |
| --- | --- | --- |
| Appointments | `Appointment.java`, `AppointmentService.java` | `AppointmentTest.java`, `AppointmentServiceTest.java` |
| Contacts | `Contact.java`, `ContactService.java` | `ContactTest.java`, `ContactServiceTest.java` |
| Tasks | `Task.java`, `TaskService.java` | `TaskTest.java`, `TaskServiceTest.java` |

The services demonstrate basic object management and field-validation rules. The tests use **JUnit Jupiter (JUnit 5)**, including test fixtures and assertions for expected and invalid inputs.

## Technology

- Java
- JUnit 5 (Jupiter)

## Running the tests

This repository contains standalone Java source and test files, but **does not currently include a Maven or Gradle build configuration**.

To run the tests locally, open the project in a Java IDE, configure a Java JDK and JUnit 5 as a test dependency, then run the `*Test.java` classes with the IDE's JUnit test runner. The exact Java version and test dependency versions have not been pinned in this repository.

## Engineering takeaways

- Keep domain objects and their managing services separate.
- Validate required fields and constraints.
- Test normal inputs and invalid or boundary cases.
- Use repeatable unit tests to detect regressions when implementation details change.

## Scope and limitations

This is a focused educational implementation, **not** a deployed web application or security-audited product. The repository does not currently demonstrate authentication, penetration testing, CI/CD pipelines, integration testing, or end-to-end testing. These are potential future extensions, not completed features.

For a broader look at my work, see my [GitHub profile](https://github.com/xtyledan) and [graduate computer science portfolio](https://github.com/xtyledan/ms-computer-science-coursework).
