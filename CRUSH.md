# Development Guide

## Build Commands
```bash
# No explicit build required for ZSH themes
```

## Lint Commands
```bash
# No specific linter configured
# Manual review of syntax and logic is sufficient
```

## Test Commands
```bash
# Testing involves manual verification in a ZSH environment
# To test a single aspect, temporarily modify the theme to highlight changes
```

## Code Style Guidelines

### General
- Follow standard ZSH scripting conventions
- Use 2-space indentation for consistency
- Maintain clear comments for complex logic
- Adhere to the existing naming conventions for variables and functions

### Imports
- No external dependencies; all code is self-contained within the theme file

### Formatting
- Use consistent spacing around operators and after commas
- Align related assignments for readability when appropriate

### Types/Naming
- Use UPPER_CASE for global variables and configuration options
- Prefix internal functions with `headline-` to avoid namespace conflicts
- Use snake_case for local variables within functions

### Error Handling
- Check command exit codes where necessary
- Gracefully handle cases where commands might fail (e.g., git operations)

### Additional Notes
- Theme customizations should be made via environment variables as documented
- Ensure all ANSI escape sequences are properly terminated with `%{%}`
- Optimize loops and string operations for performance in interactive shells