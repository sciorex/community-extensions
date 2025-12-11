# Scientific Research Workflow

A comprehensive multi-agent workflow for conducting rigorous, reproducible scientific research from initial question through final synthesis.

## Overview

The Scientific Research Workflow automates the complete research lifecycle:

1. **Research Request** - User submits a research question or topic
2. **Orchestration** - Research orchestrator scopes the work and creates tracking tickets
3. **Literature Review** - Researcher agent gathers and synthesizes existing knowledge
4. **Hypothesis Generation** - Generates testable, falsifiable hypotheses
5. **Experiment Planning** - Designs rigorous experimental protocols
6. **Experiment Execution** - Runs experiments with proper checkpointing
7. **Validation** - Validates findings at scale across conditions
8. **Synthesis** - Compiles comprehensive final reports

## Flow Diagram

```
┌─────────────────┐
│ Research Request│
│    (Trigger)    │
└────────┬────────┘
         │
         ▼
┌─────────────────┐
│    Research     │
│   Orchestrator  │──────────────────────────────┐
└────────┬────────┘                              │
         │                                       │
         ▼                                       │
┌─────────────────┐                              │
│  Approve Scope  │◄─────────┐                   │
│     (Wait)      │          │ Revise            │
└────────┬────────┘          │                   │
         │ Approved          │                   │
         ▼                   │                   │
┌─────────────────┐          │                   │
│   Literature    │──────────┘                   │
│     Review      │                              │
└────────┬────────┘                              │
         │                                       │
         ▼                                       │
┌─────────────────┐                              │
│    Hypothesis   │                              │
│    Generator    │                              │
└────────┬────────┘                              │
         │                                       │
         ▼                                       │
┌─────────────────┐     Skip to Synthesis        │
│ Approve & Test? │─────────────────────────────►│
└────────┬────────┘                              │
         │ Run Experiments                       │
         ▼                                       │
┌─────────────────┐                              │
│   Experiment    │◄─────────┐                   │
│     Planner     │          │ Revise            │
└────────┬────────┘          │                   │
         │                   │                   │
         ▼                   │                   │
┌─────────────────┐          │                   │
│ Approve Plan?   │──────────┘                   │
└────────┬────────┘                              │
         │ Execute                               │
         ▼                                       │
┌─────────────────┐                              │
│   Experiment    │                              │
│    Executor     │                              │
└────────┬────────┘                              │
         │                                       │
         ▼                                       │
┌─────────────────┐    Refuted/Inconclusive     │
│   Supported?    │─────────────────────────────►│
└────────┬────────┘                              │
         │ Supported                             │
         ▼                                       │
┌─────────────────┐     Skip Validation          │
│   Validate?     │─────────────────────────────►│
└────────┬────────┘                              │
         │ Validate                              │
         ▼                                       │
┌─────────────────┐                              │
│    Verifier     │                              │
└────────┬────────┘                              │
         │                                       │
         ▼                                       │
┌─────────────────┐◄─────────────────────────────┘
│   Synthesizer   │
└────────┬────────┘
         │
         ▼
┌─────────────────┐
│ Research Complete│
└─────────────────┘
```

## Required Agents

| Agent | Purpose |
|-------|---------|
| [research-orchestrator](../agents/scientific-research/research-orchestrator.yaml) | Scopes research, creates tracking tickets, orchestrates workflow |
| [researcher](../agents/researcher.yaml) | Conducts literature review, synthesizes findings |
| [hypothesis-generator](../agents/scientific-research/hypothesis-generator.yaml) | Generates testable hypotheses from research |
| [experiment-planner](../agents/scientific-research/experiment-planner.yaml) | Designs rigorous experimental protocols |
| [experiment-executor](../agents/scientific-research/experiment-executor.yaml) | Implements and runs experiments |
| [verifier](../agents/scientific-research/verifier.yaml) | Validates findings at scale |
| [synthesizer](../agents/scientific-research/synthesizer.yaml) | Compiles final reports |

## Key Features

### Human-in-the-Loop Approvals

The workflow includes multiple approval gates:
- **Scope Approval** - Review research scope before proceeding
- **Research Review** - Approve literature findings before hypothesis generation
- **Hypothesis Selection** - Choose which hypotheses to test
- **Experiment Approval** - Review experiment design before execution
- **Validation Decision** - Decide whether to validate at scale

### Ticket Integration

The workflow integrates with Sciorex's ticketing system:
- Creates an **Epic** for the overall research goal
- Creates **Phase Tickets** for each stage of research
- Links dependencies between tickets
- Updates status as work progresses
- Attaches results and reports to tickets

### Checkpointing & Recovery

Experiments implement proper checkpointing:
- Saves progress after each condition
- Can resume from failures
- Stores partial results incrementally
- Supports long-running experiments

### Statistical Rigor

The workflow ensures scientific validity:
- Multiple random seeds (minimum 5)
- Proper control/baseline conditions
- Statistical significance testing
- Effect size calculation
- Confidence intervals

## Usage

### Triggering the Flow

The flow is triggered when a ticket with type `research` is created:

```yaml
triggerType: ticket-created
ticketType: research
```

Or run manually from the Flow Editor.

### Input Variables

| Variable | Description |
|----------|-------------|
| `request` | The research question or topic |
| `context` | Additional context or constraints |
| `domain` | Research domain (e.g., "machine-learning") |

### Output

The flow produces:
- **Epic** with all research findings
- **Phase Tickets** documenting each stage
- **Experiment Reports** with statistical analysis
- **Final Report** (`FINAL_REPORT.md`) synthesizing conclusions
- **Artifacts** (code, data, plots) in workspace

## Example Research Topics

- "Investigate effectiveness of different attention mechanisms for sequence modeling"
- "Research best practices for API rate limiting and compare approaches"
- "Analyze caching strategies for GraphQL resolvers and measure performance"
- "Explore novel approaches to code generation using tree-structured models"

## Customization

### Modifying the Flow

The flow can be customized in the Flow Editor:
- Add/remove approval gates
- Adjust condition thresholds
- Add parallel branches
- Modify agent configurations

### Adjusting Agents

Each agent can be customized:
- Modify system prompts for domain-specific needs
- Adjust temperature for more/less creative outputs
- Configure tool permissions
- Add custom MCP servers

## Best Practices

1. **Clear Research Questions** - Start with specific, well-defined questions
2. **Scope Appropriately** - Use the orchestrator's clarifying questions
3. **Review Carefully** - Use approval gates to ensure quality
4. **Document Everything** - The workflow maintains full audit trail
5. **Iterate** - Research often requires multiple cycles

## Related Resources

- [Flow Editor Documentation](https://docs.sciorex.com/features/flows)
- [Agent Configuration](https://docs.sciorex.com/features/agents)
- [Ticketing System](https://docs.sciorex.com/features/ticketing)
