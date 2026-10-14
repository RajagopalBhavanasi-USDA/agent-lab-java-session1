🌐 [Português (BR)](README.pt_BR.md) | [Español](README.es.md)

# 🎲 Soc Ops

**A social bingo game—and a hands-on GitHub Copilot Agent lab.**

Bring an in-person mixer to life: find people who match the prompts on your card, mark each discovery, and race to five in a row. Along the way, use VS Code and GitHub Copilot Agent Mode to turn a simple Spring Boot app into your own memorable experience.

[🎮 Play the live demo](https://copilot-dev-days.github.io/agent-lab-java/) · [📚 Start the lab](workshop/GUIDE.md) · [🇧🇷 Português](README.pt_BR.md) · [🇪🇸 Español](README.es.md)

---

## Build something worth playing

In about an hour, you will practice the workflow behind an AI-assisted product iteration:

- **Set the context** so an agent understands the codebase and your goals.
- **Design with intention** and guide an agent toward a distinctive interface.
- **Create a custom Quiz Master** for bingo prompts that fit your group.
- **Ship features confidently** with multi-agent, test-driven development.

> **Stack:** Java 21 · Spring Boot 3.4 · Maven · Thymeleaf · **Level:** Intermediate · **Format:** In-person workshop

## Start the lab

| Part | Title |
|------|-------|
| [**00**](workshop/00-overview.md) | Overview & Checklist |
| [**01**](workshop/01-setup.md) | Setup & Context Engineering |
| [**02**](workshop/02-design.md) | Design-First Frontend |
| [**03**](workshop/03-quiz-master.md) | Custom Quiz Master |
| [**04**](workshop/04-multi-agent.md) | Multi-Agent Development |

> 📝 Lab guides are also available in the [`workshop/`](workshop/) folder for offline reading.

---

## Get playing

### Prerequisites

- [Java 21 JDK](https://adoptium.net/) or higher
- [Apache Maven 3.9+](https://maven.apache.org/) (or use the included Maven Wrapper)

### Run locally

```bash
cd socops
./mvnw spring-boot:run
```

Then open [http://localhost:8080](http://localhost:8080), invite a few people over, and start marking your card.

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

## Share your version

Give the game a theme, tailor the questions to your event, and publish it for your group. The project deploys automatically to GitHub Pages on push to `main`.
