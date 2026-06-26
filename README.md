This (constitution)[https://github.com/maxsonferovante/proposal-python-constitution-spec-kit/blob/main/constitution.md] defines a set of technical and organizational rules to guide the development of a modern Python project using the [Spec Kit](https://github.com/github/spec-kit).

It mandates that the code adhere to Python best practices, including PEP 8, PEP 257, type hints, the use of `pyproject.toml`, automated testing, linting, formatting, static analysis, and atomic commits. The primary focus is ensuring readability, simplicity, maintainability, and predictability.

The proposed architecture follows Clean Architecture principles, clearly separating responsibilities across the domain, application, interface, and infrastructure layers. Business logic must remain isolated from frameworks, databases, external APIs, and technical details. The domain layer must be independent, while the infrastructure layer implements contracts defined by the application.

The constitution also reinforces OOP and SOLID principles, advocating for classes with clear responsibilities, composition over excessive inheritance, the use of protocols, small abstractions, and dependency on interfaces rather than concrete implementations.

Furthermore, it defines best practices for design patterns such as Repository, Unit of Work, Factory, Strategy, Adapter, Facade, Command, Specification, and Domain Events. These patterns should be employed only when they enhance clarity, testability, or component substitutability.

Regarding persistence, the constitution mandates that SQLAlchemy usage be restricted to the infrastructure layer. The application must access data via repositories and the Unit of Work pattern, preventing the leakage of sessions, ORM models, or queries outside that layer.

It also establishes standards for testing, error handling, security, configuration, observability, performance, documentation, ADRs, code review, and minimum quality requirements prior to merging. All significant changes must pass quality gates, including checks for formatting, linting, typing, testing, documentation, and the preservation of architectural boundaries. Finally, the constitution formalizes the use of the Spec Kit workflow:

```text
/speckit.constitution
/speckit.specify
/speckit.plan
/speckit.tasks
/speckit.implement
```

Each stage must adhere to the defined principles, ensuring that specifications, plans, tasks, and implementations are coherent, testable, well-documented, and aligned with the project architecture.

(Download)[https://github.com/maxsonferovante/proposal-python-constitution-spec-kit/blob/main/constitution.md]
