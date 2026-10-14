🌐 [Português (BR)](README.pt_BR.md) | [Español](README.es.md)

# Soc Ops

Soc Ops is a social bingo experience for in-person mixers, workshops, and team events.
Participants match prompts with real people in the room and race to complete five-in-a-row.

[Start the Lab Guide](workshop/GUIDE.md)

---

## Why This Project Is Fun

- Fast to run locally and easy to customize.
- Great demo app for Spring Boot + Thymeleaf fundamentals.
- Built for agent-driven development workshops.
- Includes structured labs from setup to multi-agent workflows.

---

## Quick Start

### Prerequisites

- [Java 21 JDK](https://adoptium.net/) or higher
- Maven 3.9+ (or use the included Maven Wrapper)

### Run Locally

```bash
cd socops
./mvnw spring-boot:run
```

Open http://localhost:8080

### Build

```bash
cd socops
./mvnw clean package
```

### Test

```bash
cd socops
./mvnw test
```

---

## Workshop Journey

| Part | Focus |
|------|-------|
| [00](workshop/00-overview.md) | Overview and checklist |
| [01](workshop/01-setup.md) | Setup and context engineering |
| [02](workshop/02-design.md) | Design-first frontend |
| [03](workshop/03-quiz-master.md) | Custom quiz-master agent |
| [04](workshop/04-multi-agent.md) | Multi-agent development |
| [05](workshop/05-complete.md) | Wrap-up and completion |

Browse all guides in [workshop](workshop/).

---

## Project Map

- Application code: [socops](socops/)
- UI template: [socops/src/main/resources/templates/game.html](socops/src/main/resources/templates/game.html)
- Styles: [socops/src/main/resources/static/css/app.css](socops/src/main/resources/static/css/app.css)
- API/controller: [socops/src/main/java/com/socops/web/BingoRestController.java](socops/src/main/java/com/socops/web/BingoRestController.java)
- Tests: [socops/src/test/java/com/socops/service/BoardAssemblerTests.java](socops/src/test/java/com/socops/service/BoardAssemblerTests.java)
- Documentation site assets: [docs](docs/)

---

## Deployment Note

The docs site deploys automatically to GitHub Pages when changes are pushed to main.
