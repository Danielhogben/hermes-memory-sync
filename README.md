# hermes-memory-sync

**Persistent memory management for Hermes agent with versioning and cross-session sync**

## Overview

Part of the Hermes agent ecosystem - a collection of tools and skills for AI agent workflows.

This skill enables persistent memory storage with versioning, query capabilities, and cross-session synchronization for the Hermes AI agent framework.

## Installation

Copy the SKILL.md to your Hermes skills directory:

```bash
mkdir -p ~/.hermes/skills/hermes-memory-sync
cp SKILL.md ~/.hermes/skills/hermes-memory-sync/SKILL.md
```

## Features

- **Store Facts**: Add persistent memories across categories (user, project, system, workflow, decision)
- **Query Memory**: Retrieve relevant memories using natural language queries
- **Version Control**: Track changes to memories over time
- **Cross-Session Sync**: Share memory across different agent sessions
- **GitHub Integration**: Optional GitHub sync for team sharing

## Quick Start

```bash
# Add a memory
memory add user "Donn prefers concise responses and direct action"

# Query memories
memory query "user preferences"

# List project memories  
memory list --project deer-flow
```

## Integration

Works with:
- `hermes-task-tracker` for project context
- `hermes-doc-generator` for capturing decisions
- `hermes-code-analyzer` for storing patterns

## GitHub

- https://github.com/Danielhogben/hermes-memory-sync

## License

MIT
