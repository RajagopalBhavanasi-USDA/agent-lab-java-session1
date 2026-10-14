# Copilot Workspace Instructions

## Scope
- Prioritize changes in socops.
- Do not edit docs or workshop content unless explicitly requested.

## Build And Run Rules
- Use Java 21 for all Maven commands.
- Run the Maven wrapper from socops.
- In PowerShell, use ; instead of &&.
- Standard commands from workspace root:
  - cd socops; ./mvnw clean package
  - cd socops; ./mvnw test
  - cd socops; ./mvnw spring-boot:run

## Mandatory Development Checklist
- [ ] Keep changes minimal and task-focused.
- [ ] Build succeeds (clean package).
- [ ] Relevant tests pass.
- [ ] App starts and responds on localhost for runtime/UI changes.
- [ ] Follow existing naming/style; add comments only for non-obvious logic.
- [ ] Avoid new dependencies unless required by the task.

## Quick Code Map
- App code: socops/src/main/java/com/socops
- Templates: socops/src/main/resources/templates
- Static assets: socops/src/main/resources/static
- Tests: socops/src/test/java/com/socops
