# Contributing to NGCC

Thank you for your interest in contributing to NGCC! This document provides guidelines and instructions for contributing.

## Code of Conduct

By participating in this project, you agree to abide by our [Code of Conduct](./CODE_OF_CONDUCT.md).

## How to Contribute

### Reporting Bugs

- Search [existing issues](https://github.com/assistanz/angular-carbon-components/issues) before opening a new one.
- Use the bug report template and include:
  - Angular version
  - `ngcc` version
  - Steps to reproduce
  - Expected vs actual behavior

### Suggesting Features

- Open a [feature request issue](https://github.com/assistanz/angular-carbon-components/issues/new) describing the use case and expected behavior.

### Submitting Pull Requests

1. Fork the repository and create a branch from `main`.
2. Install dependencies: `npm install`
3. Make your changes following the guidelines below.
4. Add or update tests for your changes.
5. Run tests: `npm run test`
6. Run Storybook to verify visual changes: `npm run storybook`
7. Submit a pull request against `main`.

## Development Setup

```bash
# Clone your fork
git clone https://github.com/<your-username>/angular-carbon-components.git
cd angular-carbon-components

# Install dependencies
npm install

# Run Storybook
npm run storybook

# Run Precheck
npm run precheck

# Build the library
npx ng build ngcc
```

## Coding Guidelines

- Use Angular 20+ standalone components with signals (`input()`, `output()`, `signal()`, `computed()`).
- Set `changeDetection: ChangeDetectionStrategy.OnPush` on all components.
- Follow the [Angular style guide](https://angular.dev/style-guide).
- Use native control flow (`@if`, `@for`, `@switch`) instead of structural directives.
- Implement `ControlValueAccessor` for form components.
- All components must meet WCAG 2.1 AA accessibility standards.
- Include `vitest-axe` accessibility tests in every component spec file.

## Commit Messages

Use clear, descriptive commit messages:

```
[Task-ID: #XXXXX] Short description of the change

Message/Note: Additional context about what was changed and why.
```

## License

By contributing, you agree that your contributions will be licensed under the [MIT License](./LICENSE).
