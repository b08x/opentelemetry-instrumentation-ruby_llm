```markdown
# opentelemetry-instrumentation-ruby_llm Development Patterns

> Auto-generated skill from repository analysis

## Overview
This skill teaches you the development patterns, coding conventions, and workflows used in the `opentelemetry-instrumentation-ruby_llm` Ruby codebase. You'll learn how to structure files, import and export modules, and write and run tests in alignment with the repository's established practices.

## Coding Conventions

### File Naming
- Use **CamelCase** for file names.
  - Example: `OpenTelemetryInstrumentation.rb`, `LlmTracer.rb`

### Import Style
- Use **relative imports** to include other files or modules.
  - Example:
    ```ruby
    require_relative 'LlmTracer'
    ```

### Export Style
- Use **named exports** for modules and classes.
  - Example:
    ```ruby
    module OpenTelemetryInstrumentation
      class LlmTracer
        # ...
      end
    end
    ```

### Commit Messages
- Commit messages are freeform, with no strict prefixing.
- Average commit message length is around 67 characters.

## Workflows

### Adding a New Instrumentation Module
**Trigger:** When you need to add support for a new LLM or service.
**Command:** `/add-instrumentation`

1. Create a new CamelCase Ruby file for your module.
2. Use relative imports to include dependencies.
3. Export your module/class using named exports.
4. Write corresponding tests in a `*.test.*` file.
5. Commit your changes with a clear, descriptive message.

### Updating an Existing Module
**Trigger:** When modifying or enhancing an existing instrumentation module.
**Command:** `/update-module`

1. Locate the relevant CamelCase file.
2. Make your changes, following the import/export conventions.
3. Update or add tests as needed.
4. Commit your changes with a descriptive message.

### Running Tests
**Trigger:** Before merging or after making changes.
**Command:** `/run-tests`

1. Identify all `*.test.*` files.
2. Use the project's preferred testing tool (framework not specified; consult project docs or `README` if available).
3. Run the tests and ensure all pass.
4. Address any failures before proceeding.

## Testing Patterns

- Test files follow the pattern: `*.test.*`
  - Example: `LlmTracer.test.rb`
- The testing framework is not explicitly specified; check for documentation or scripts in the project for details.
- Place tests alongside or near the code they cover, using the same CamelCase naming convention.

## Commands
| Command              | Purpose                                              |
|----------------------|------------------------------------------------------|
| /add-instrumentation | Scaffold a new instrumentation module                |
| /update-module       | Update or enhance an existing module                 |
| /run-tests           | Run all test files in the repository                 |
```
