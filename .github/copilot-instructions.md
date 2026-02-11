# Copilot Instructions for JavaScript Project

## Project Overview
This is a minimal JavaScript web project with core logic in `rev.js`. The project implements numeric algorithms as standalone JavaScript functions with HTML/CSS templates for UI integration.

## Architecture & Key Components

### Core Logic (`rev.js`)
- **Purpose**: Contains reusable JavaScript algorithms and utilities
- **Current Pattern**: Imperative number reversal algorithm using modulo arithmetic
- **Convention**: Functions should be self-contained with minimal dependencies; avoid global state where possible
- **Important**: Console output is used for testing/validation (consider replacing with proper function returns)

### Front-end Structure
- `index.html`: Web page entry point (currently empty - under development)
- `script.css`: Styling (currently empty - under development)
- **Pattern**: Keep JavaScript separate from HTML; load scripts via `<script src="rev.js"></script>` tags

## Development Workflow

### Running Code
- Direct execution: `node rev.js` in PowerShell to test algorithm logic
- Browser testing: Open `index.html` in a browser (once populated) to test DOM integration
- No build system currently configured (plain JavaScript)

### Testing Approach
- **Current**: Algorithm output validated via `console.log()`
- **Recommendation**: Refactor algorithm returns from `console.log()` to explicit return statements for testability
- Functions should return values rather than print them

## Project Conventions

### JavaScript Style
- Use `let`/`const` for variable declarations (no `var`)
- Use `Math.floor()` for integer division operations
- Variable naming: descriptive (`rem`, `rev`, `a` are temporary but context-clear)

### Algorithm Pattern
- Iterative loops for numeric transformations (avoid recursion for now)
- Modulo arithmetic for digit manipulation
- Floor division for integer operations

## Common Tasks

- **Add new algorithms**: Create functions in `rev.js` with explicit return statements
- **Display results in UI**: Parse `rev.js` output and bind to HTML elements
- **Style components**: Add CSS classes to `index.html` and define in `script.css`

## Known Issues & Improvements
- Algorithm uses console.log instead of returning values - refactor for better testability
- No error handling for negative numbers or edge cases
- HTML/CSS files are empty stubs - awaiting implementation
