# Changelog

All notable changes to this project will be documented in this file.

The format is based on [Keep a Changelog](https://keepachangelog.com/en/1.1.0/),
and this project adheres to [Semantic Versioning](https://semver.org/spec/v2.0.0.html).

## [Unreleased]

### Added

- Button component with primary, secondary, tertiary, danger, and ghost variants
- Checkbox component with reactive forms support (ControlValueAccessor)
- Input (text, number) and Textarea components with validation states
- Dropdown component with single/multi-select, search, and keyboard navigation
- Datepicker component with calendar overlay
- Table component with sorting, filtering, pagination, and row selection
- Pagination component
- Notification and Toast components with service-based API
- Modal component with focus trapping
- Tooltip component with configurable placement
- Tabs component with router integration support
- Accordion component
- Skeleton loading component
- Icon component with built-in Carbon icon set
- Charts integration (Bar, Line, Donut, Pie, etc.) via @carbon/charts
- Gauge Chart component
- Theme Switcher (white, g10, g90, g100)
- Color Theme Service with dynamic brand color support and WCAG contrast validation
- WCAG 2.1 AA accessibility tests (vitest-axe) for all components
- Storybook documentation for all components
- CI pipeline with build, test, and coverage

### Technical

- Angular 20+ with standalone components and signals
- OnPush change detection on all components
- Zoneless-compatible
- Tree-shakeable (`sideEffects: false`)

## [0.0.1] - 2026-02-10

- Initial pre-release
