# yashwant-plugin

A Claude Code plugin for Flutter/Dart code reviews. Built for the Heidi team.

## Skills

### `/yashwant-plugin:code-review`

Reviews Flutter/Dart code for bugs, best practices, style, and performance issues.

**Usage:**
```
/yashwant-plugin:code-review lib/feat/home/widgets/listing_widget.dart
```
Or just ask: *"review this file"* and Claude will trigger it automatically.

**Checks:**
- Null safety violations and unhandled errors
- Flutter widget lifecycle and setState usage
- Dart naming conventions and const constructors
- Performance (unnecessary rebuilds, missing list keys)
- Security (hardcoded secrets, unsafe HTTP)

## Installation

### Add this plugin to Claude Code

```
/plugin install yashwant1999/yashwant-plugin
```

### Or add as a marketplace

```
/plugin marketplace add yashwant1999/yashwant-plugin
```

## Adding More Skills

To add a new skill, create a folder under `skills/` with a `SKILL.md` file:

```
skills/
└── my-skill/
    └── SKILL.md
```

Then bump the version in `.claude-plugin/plugin.json` and push.
