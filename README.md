# Java Service Testing and Software Quality

[![Java service tests](https://github.com/xtyledan/Java-Service-Testing-Appointment-Contact-Task-Management/actions/workflows/java-tests.yml/badge.svg)](https://github.com/xtyledan/Java-Service-Testing-Appointment-Contact-Task-Management/actions/workflows/java-tests.yml)

**A test-driven Java learning project:** implement three small domain services, enforce input constraints, and run JUnit 5 tests with a reproducible Maven build.

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

## Run the tests

Requirements: Java 11 or newer and Apache Maven 3.9+. GitHub Actions runs the suite on Temurin Java 17.

```bash
git clone https://github.com/xtyledan/Java-Service-Testing-Appointment-Contact-Task-Management.git
cd Java-Service-Testing-Appointment-Contact-Task-Management
mvn test
```

The project retains its original flat Java source layout. The supplied `pom.xml` separates `*Test.java` files during compilation and uses JUnit Jupiter with Maven Surefire. [View the automated test runs](https://github.com/xtyledan/Java-Service-Testing-Appointment-Contact-Task-Management/actions/workflows/java-tests.yml).

**Example:** The `ContactServiceTest.java` tests contact creation and expected field constraints. `AppointmentServiceTest.java` and `TaskServiceTest.java` cover their corresponding domain services. These are unit tests, not a live web demo; no application screenshot would be representative.

## Engineering takeaways

- Keep domain objects and their managing services separate.
- Validate required fields and constraints.
- Test normal inputs and invalid or boundary cases.
- Use repeatable unit tests to detect regressions when implementation details change.

## Scope and limitations

This is a focused educational implementation, **not** a deployed web application or security-audited product. The repository does not demonstrate authentication, penetration testing, integration testing, or end-to-end testing. A GitHub Actions CI workflow now runs the unit tests. These are potential future extensions, not completed features.

For a broader look at my work, see my [GitHub profile](https://github.com/xtyledan) and [graduate computer science portfolio](https://github.com/xtyledan/ms-computer-science-coursework).

## License

[MIT License](LICENSE).
