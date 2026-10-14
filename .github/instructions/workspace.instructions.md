---
applyTo: "**"
description: Workspace-wide guidance for developing and validating the Soc Ops Spring Boot project.
---

# Workspace Instructions

## Project Scope
- Primary application code lives in socops.
- Treat docs and workshop content as instructional material unless a task explicitly asks to update them.
- Keep changes focused and minimal; avoid broad refactors unless requested.

## Runtime And Toolchain
- Use Java 21 for all build, test, and run operations.
- If Java 17 is active by default, set JAVA_HOME to the local JDK 21 path before running Maven commands.
- Use the Maven wrapper from the socops folder.

## Windows PowerShell Notes
- Use semicolon separators in task commands, not &&.
- Prefer commands in this form from workspace root:
  - cd socops; ./mvnw clean package
  - cd socops; ./mvnw test
  - cd socops; ./mvnw spring-boot:run

## Verification Workflow
- Build: run clean package and confirm BUILD SUCCESS.
- Tests: run test and confirm all tests pass.
- Run: start spring-boot:run and verify app responds on localhost.
- If port 8080 is in use, either stop the conflicting process or run on a temporary alternate port for verification.

## Code Organization
- Java sources: socops/src/main/java/com/socops
- Templates: socops/src/main/resources/templates
- Static assets: socops/src/main/resources/static
- Tests: socops/src/test/java/com/socops

## Editing Guidelines
- Preserve existing naming and style conventions.
- Add comments only when logic is non-obvious.
- Avoid introducing new dependencies unless needed for the requested task.
- When editing UI, align with existing utility CSS usage in app.css.

## Done Criteria
- Requested change is implemented.
- Project builds successfully with Java 21.
- Relevant tests pass.
- Runtime behavior is validated locally when applicable.
