---
name: hermes-memory-sync
description: Persistent memory management for Hermes - sync, version, and query agent memory across sessions
---

# Hermes Memory Sync

Persistent memory management with versioning, query capabilities, and cross-session sync for Hermes agent.

## Memory Operations

### Store Facts
Add important facts to persistent memory:
```
memory add user "Donn prefers concise responses and direct action"
memory add project "Deer-flow requires Docker, TAVILY_API_KEY, JINA_API_KEY"
```

### Query Memory
Retrieve relevant memories:
```
memory query "user preferences"
memory query "project requirements"
```

## Commands

### Add Memory
```bash
hermes-memo add <category> "<key>: <value>" --context "<description>"
```

### Find Memory
```bash
hermes-memo find <query>
hermes-memo list --project deer-flow
```

## Memory Categories

- **user**: Personal info, preferences, timezone, role
- **project**: Project requirements, dependencies, build commands
- **system**: Environment facts, tool versions, paths
- **workflow**: Procedures, patterns, recurring tasks
- **decision**: Key decisions and their rationale

## Integration

Works with:
- `hermes-task-tracker` for project context
- `hermes-doc-generator` for capturing decisions
- `hermes-code-analyzer` for storing patterns

## Files

- `~/.hermes/memory/` - Local memory store
- `~/.hermes/memory/memory.json` - Main memory database
