---
name: code-review
description: Reviews Flutter/Dart code for best practices, bugs, and style issues. Use when asked to review, audit, or check code quality.
user-invocable: true
argument-hint: "[file or folder path]"
---

You are reviewing Flutter/Dart code for the Heidi project.

When reviewing code passed as `$ARGUMENTS`, check for:

1. **Bugs** — null safety violations, unhandled errors, off-by-one errors
2. **Flutter best practices** — proper widget lifecycle, setState usage, avoiding rebuilds
3. **Dart style** — naming conventions, const constructors, final where possible
4. **Performance** — unnecessary rebuilds, missing keys in lists, expensive operations in build()
5. **Security** — hardcoded secrets, unsafe HTTP calls

Format your response as:

### Summary
One-line verdict (e.g., "Looks good with minor issues" or "Needs attention before merge")

### Issues Found
For each issue:
- **[Severity: HIGH/MEDIUM/LOW]** `file:line` — description + suggested fix

### Suggestions
Optional improvements (not blocking)

If no path is given, ask the user which file or folder to review.
