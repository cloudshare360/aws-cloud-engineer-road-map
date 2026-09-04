# Agent Memory

Agent memory files for the AWS Cloud Engineer roadmap project.

## Memory Directory

```
.kilo/memory/
├── project.md          # Project facts and structure
├── environment.md      # Environment commands and paths
├── corrections.md      # Corrections and decisions
├── project-memory.md   # Additional project memory
└── session-summary.md  # Session summaries
```

## Memory Types

- **project.md**: Durable project facts, structure, conventions
- **environment.md**: Commands, paths, tooling setup
- **corrections.md**: Past corrections and decisions
- **project-memory.md**: Additional memory entries
- **session-summary.md**: Session handoff digests

## Usage

Memory is auto-loaded by Kilo at session start. Use `kilo_memory_recall` to search memory and `kilo_memory_save` to add new entries.

## Adding New Memory

Use `kilo_memory_save` with action `remember` to add durable facts. Use `correct` to fix stale memory. Use `forget` to remove outdated entries.
