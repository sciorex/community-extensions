# Contributing to Sciorex Community

Thank you for your interest in contributing to the Sciorex community repository! This document provides guidelines for contributing agents and flows.

## Table of Contents

- [Getting Started](#getting-started)
- [Contribution Types](#contribution-types)
- [Creating an Agent](#creating-an-agent)
- [Creating a Flow](#creating-a-flow)
- [Submission Process](#submission-process)
- [Review Criteria](#review-criteria)
- [Style Guide](#style-guide)

## Getting Started

1. **Fork** this repository
2. **Clone** your fork locally
3. **Test** your contribution in Sciorex
4. **Submit** a pull request

### Prerequisites

- A working Sciorex installation
- Familiarity with YAML (for agents) and JSON (for flows)
- Understanding of the Sciorex agent/flow architecture

## Contribution Types

### New Agent

Create a new AI agent that performs a specific task.

### New Flow

Create a new automated workflow combining multiple agents.

### Improvement

Enhance an existing agent or flow with bug fixes or new capabilities.

### Documentation

Improve documentation, examples, or add translations.

## Creating an Agent

### Agent File Structure

Create a YAML file in the `agents/` directory:

```yaml
id: my-agent-id          # Unique, lowercase, hyphenated
name: My Agent Name      # Human-readable name
description: |           # Clear description of what it does
  A concise description of your agent's purpose and capabilities.
icon: "emoji"            # Single emoji representing the agent
version: "1.0.0"         # Semantic version

systemPrompt: |
  You are a [role]. Your job is to [primary task].

  When working:
  1. [Step 1]
  2. [Step 2]
  3. [Step 3]

  Guidelines:
  - [Guideline 1]
  - [Guideline 2]

  Output format:
  Provide your response in the following JSON structure:
  {
    "field1": "description",
    "field2": "description"
  }

adapter: claude-code
model: claude-sonnet-4-20250514

inputSchema:
  type: object
  properties:
    inputField:
      type: string
      description: Description of this input
  required:
    - inputField

outputSchema:
  type: object
  properties:
    outputField:
      type: string
  required:
    - outputField

allowedTools:
  - Read
  - Glob
  - Grep
  # Add other tools as needed

autoApprove:
  - Read
  - Glob
  - Grep
```

### Agent Guidelines

1. **Unique ID**: Use lowercase letters and hyphens (e.g., `code-formatter`)
2. **Clear Purpose**: Each agent should have a single, well-defined purpose
3. **Structured Output**: Define a clear JSON output schema
4. **Minimal Permissions**: Only request tools the agent actually needs
5. **Good Prompts**: Write clear, detailed system prompts

### Available Tools

| Tool | Description |
|------|-------------|
| `Read` | Read file contents |
| `Glob` | Find files by pattern |
| `Grep` | Search file contents |
| `Write` | Write to files |
| `Edit` | Edit existing files |
| `Bash` | Execute shell commands |

## Creating a Flow

### Flow File Structure

Create a JSON file in the `flows/` directory:

```json
{
  "id": "my-flow-id",
  "name": "My Flow Name",
  "description": "Description of what this flow does",
  "nodes": [
    {
      "id": "trigger-1",
      "type": "trigger",
      "position": { "x": 250, "y": 50 },
      "data": {
        "type": "trigger",
        "label": "Manual Trigger",
        "triggerType": "manual",
        "triggerConfig": {}
      }
    }
    // ... more nodes
  ],
  "edges": [
    {
      "id": "edge-1",
      "source": "trigger-1",
      "target": "next-node"
    }
  ],
  "variables": {},
  "labelIds": [],
  "version": "1.0.0",
  "author": "Your Name",
  "createdAt": "2025-01-01T00:00:00Z",
  "updatedAt": "2025-01-01T00:00:00Z"
}
```

### Flow Guidelines

1. **Document Dependencies**: List all required agents in `requiredAgents`
2. **Logical Layout**: Arrange nodes in a clear, readable manner
3. **Error Handling**: Include condition nodes for error cases
4. **Clear Labels**: Use descriptive labels for all nodes

## Submission Process

### 1. Update index.json

Add your contribution to `index.json`:

For agents:
```json
{
  "id": "my-agent",
  "name": "My Agent",
  "description": "What it does",
  "icon": "emoji",
  "version": "1.0.0",
  "author": "Your Name",
  "tags": ["tag1", "tag2"],
  "downloadUrl": "agents/my-agent.yaml",
  "updatedAt": "2025-01-01T00:00:00Z"
}
```

For flows:
```json
{
  "id": "my-flow",
  "name": "My Flow",
  "description": "What it does",
  "version": "1.0.0",
  "author": "Your Name",
  "tags": ["tag1", "tag2"],
  "downloadUrl": "flows/my-flow.json",
  "requiredAgents": ["agent-id-1"],
  "updatedAt": "2025-01-01T00:00:00Z"
}
```

### 2. Create Pull Request

1. Commit your changes with a clear message
2. Push to your fork
3. Open a pull request against `main`
4. Fill out the PR template completely

### 3. Review Process

- Maintainers will review your submission
- You may be asked to make changes
- Once approved, your contribution will be merged

## Review Criteria

Submissions are evaluated on:

| Criteria | Description |
|----------|-------------|
| **Functionality** | Does it work correctly? |
| **Usefulness** | Does it solve a real problem? |
| **Quality** | Is the code/prompt well-written? |
| **Documentation** | Is it well-documented? |
| **Originality** | Does it duplicate existing items? |
| **Security** | Are there any security concerns? |

## Style Guide

### Naming Conventions

- **Agent IDs**: `lowercase-hyphenated`
- **Flow IDs**: `lowercase-hyphenated`
- **Display Names**: Title Case

### Version Numbers

Use semantic versioning:
- **MAJOR**: Breaking changes
- **MINOR**: New features (backward compatible)
- **PATCH**: Bug fixes

### Tags

Use consistent, lowercase tags:
- `git`, `code-quality`, `testing`, `documentation`
- `automation`, `workflow`, `utility`, `analysis`

## Legal

By submitting a contribution, you agree to:

1. The [Contributor License Agreement](CLA.md)
2. License your contribution under MIT
3. The [Code of Conduct](CODE_OF_CONDUCT.md)

## Questions?

- Open a [Discussion](https://github.com/sciorex/community-extensions/discussions)
- Check existing [Issues](https://github.com/sciorex/community-extensions/issues)

Thank you for contributing!
