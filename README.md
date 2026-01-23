<p align="center">
  <img src="logo.png" alt="Sciorex Logo" width="120" />
</p>

<h1 align="center">Sciorex Community</h1>

<p align="center">
  <strong>Community-contributed agents, flows, personas, and LaTeX templates</strong><br>
  Extend Sciorex with community-built AI agents, automated workflows, council personas, and LaTeX templates
</p>

<!-- Badges -->
<p align="center">
  <a href="https://gitlab.com/sciorex/community-extensions/-/issues"><img src="https://img.shields.io/badge/issues-gitlab-orange?style=flat-square" alt="Issues"></a>
  <a href="https://gitlab.com/sciorex/community-extensions/-/merge_requests"><img src="https://img.shields.io/badge/merge_requests-gitlab-orange?style=flat-square" alt="Merge Requests"></a>
  <a href="LICENSE"><img src="https://img.shields.io/badge/license-MIT-blue?style=flat-square" alt="License"></a>
</p>

<p align="center">
  <a href="https://sciorex.com">Sciorex</a> •
  <a href="https://docs.sciorex.com">Documentation</a> •
  <a href="CONTRIBUTING.md">Contributing</a> •
  <a href="https://discord.gg/zSjPjA5j">Discord</a>
</p>

---

## Overview

This repository hosts community-contributed AI agents, automated workflows (flows), LLM Council personas, and LaTeX templates that extend Sciorex's capabilities. Users can browse, install, and update these extensions directly from within the Sciorex application.

## Contents

### Agents

#### General Purpose

| Agent | Description |
|-------|-------------|
| [git-committer](agents/git-committer.yaml) | Generates smart, contextual commit messages following conventional commit standards |
| [code-reviewer](agents/code-reviewer.yaml) | Reviews code for bugs, style issues, security vulnerabilities, and best practices |
| [codebase-researcher](agents/codebase-researcher.yaml) | Explores and analyzes codebases to understand structure, patterns, and relationships |
| [test-writer](agents/test-writer.yaml) | Generates unit and integration tests for your code |
| [doc-generator](agents/doc-generator.yaml) | Creates documentation including JSDoc comments, README files, and API docs |

#### Development Workflow Suite

Agents for structured software development with ticket tracking.

| Agent | Description |
|-------|-------------|
| [planner](agents/development-workflow/planner.yaml) | Analyzes requirements and creates implementation plans |
| [executor](agents/development-workflow/executor.yaml) | Implements code changes based on plans |
| [tester](agents/development-workflow/tester.yaml) | Creates and runs tests for implemented features |

#### Scientific Research Suite

Agents designed to work together for rigorous scientific research workflows.

| Agent | Description |
|-------|-------------|
| [research-orchestrator](agents/scientific-research/research-orchestrator.yaml) | Entry point that scopes research and creates tracking tickets |
| [researcher](agents/scientific-research/researcher.yaml) | Conducts literature review with intellectual honesty, proposes novel ideas |
| [hypothesis-generator](agents/scientific-research/hypothesis-generator.yaml) | Generates testable, falsifiable hypotheses from research findings |
| [experiment-planner](agents/scientific-research/experiment-planner.yaml) | Designs rigorous experimental protocols with statistical rigor |
| [experiment-executor](agents/scientific-research/experiment-executor.yaml) | Implements and runs experiments with checkpointing |
| [verifier](agents/scientific-research/verifier.yaml) | Validates findings at scale across conditions |
| [synthesizer](agents/scientific-research/synthesizer.yaml) | Compiles comprehensive final reports |

### Flows

| Flow | Description | Required Agents |
|------|-------------|-----------------|
| [git-workflow](flows/git-workflow.json) | Complete git workflow: review code, generate commit message, commit | git-committer, code-reviewer |
| [pr-review](flows/pr-review.json) | Automated PR review with approval gates for critical issues | code-reviewer |
| [scientific-research](flows/scientific-research/) | Complete research workflow from question to synthesis ([details](flows/scientific-research/README.md)) | research-orchestrator, researcher, hypothesis-generator, experiment-planner, experiment-executor, verifier, synthesizer |

### Personas

Council personas give AI agents specific perspectives and expertise for LLM Council discussions. Each persona defines a unique viewpoint that shapes how an agent analyzes problems and contributes to technical discussions.

| Persona | Description |
|---------|-------------|
| [The Architect](personas/architect.yaml) | Focuses on system design, patterns, and long-term architectural implications |
| [Devil's Advocate](personas/devils-advocate.yaml) | Challenges assumptions and identifies potential issues to strengthen proposals |
| [The Pragmatist](personas/pragmatist.yaml) | Focuses on practical, actionable implementation with realistic constraints |
| [The Researcher](personas/researcher.yaml) | Provides analysis, references, and evidence-based best practices |
| [The Simplifier](personas/simplifier.yaml) | Advocates for the simplest effective solution, championing KISS and YAGNI |

### LaTeX Templates

Professional LaTeX document templates for academic papers, presentations, and general-purpose documents. Templates include placeholder support for easy customization.

| Template | Description |
|----------|-------------|
| [IEEE Conference Paper](latex-templates/ieee/) | Standard IEEE conference paper template for engineering and computer science |
| [ACM Conference Paper](latex-templates/acm/) | Official ACM conference paper template (sigconf format) |
| [arXiv Preprint](latex-templates/arxiv/) | Clean template for arXiv preprints compatible with submission requirements |
| [Basic Article](latex-templates/basic-article/) | Simple article template for essays, reports, and documentation |
| [Beamer Presentation](latex-templates/beamer/) | Professional presentation template for academic and technical talks |

See [latex-templates/README.md](latex-templates/README.md) for details on template structure and contributing new templates.

## Installation

### From Sciorex App

1. Open Sciorex
2. Navigate to **Agents** or **Flows** view
3. Click **Browse Community**
4. Find the agent or flow you want
5. Click **Install**

### Manual Installation

1. Download the agent YAML, flow JSON, or persona YAML file
2. Place it in your workspace:
   - Agents: `.sciorex/community/agents/`
   - Flows: `.sciorex/community/flows/`
   - Personas: `.sciorex/community/personas/`
3. Restart Sciorex or refresh the view

## Contributing

We welcome contributions from the community! See [CONTRIBUTING.md](CONTRIBUTING.md) for guidelines.

### Quick Start

1. Fork this repository
2. Create your agent or flow
3. Test it locally in Sciorex
4. Submit a merge request

## Versioning

- Each agent and flow has its own version number
- The `index.json` has a repository version
- Use semantic versioning (MAJOR.MINOR.PATCH)

## License

This repository is licensed under the [MIT License](LICENSE).

Individual contributions retain their original copyright but must be compatible with the MIT license.

## Code of Conduct

Please read our [Code of Conduct](CODE_OF_CONDUCT.md) before participating.

## Support

- [Open an issue](https://gitlab.com/sciorex/community-extensions/-/issues) for bugs or feature requests
- [Sciorex Documentation](https://docs.sciorex.com) for questions and guides
