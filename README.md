# Dopax

Dopax is a fork of [OpenAI Codex](https://github.com/openai/codex), developed as an adaptive intelligence client for computer I/O operations, agent workflows, and project-aware execution.

The project builds on top of the Codex codebase while moving in its own direction around product design, operational workflows, and custom integrations.

## Overview

Dopax is intended to feel less like a simple chat window and more like a workspace-aware operator for engineering work.

The aim is to support real development tasks such as:

- multi-step agent workflows
- file and project awareness
- controlled command execution
- long-running task continuity
- human-in-the-loop approvals
- extensible integrations and tool layers

## Product Direction

Dopax is currently being shaped around a few core ideas:

- **Agent-native interaction**: task-oriented sessions, not just question-and-answer chat
- **Workspace awareness**: actions should stay grounded in the actual repository and local project context
- **Controlled autonomy**: the system should be able to act, while preserving clear user control over permissions and decisions
- **Operational clarity**: users should be able to understand what the agent is doing and what changed
- **Extensible foundations**: the system should evolve across models, runtimes, tools, and deployment styles

## Current Status

This repository is under active development and restructuring.

There are currently **no released packages** for this project:

- no installable binary releases
- no npm package
- no Homebrew package

At this stage, Dopax should be built and run directly from source.

## Relationship To Upstream

- Upstream repository: [`openai/codex`](https://github.com/openai/codex)
- This repository is a maintained fork with project-specific customization
- The Codex architecture and core runtime remain the technical foundation
- Some repository structure and documentation still reflect the upstream layout and will continue to be adapted for Dopax

## Local Development

The recommended way to build and run the project is from the `codex-rs` workspace:

```bash
git clone https://github.com/tensorstaff/dopax.git
cd dopax/codex-rs

cargo build
cargo run --bin codex -- "explain this codebase to me"
```

If you work on the repository regularly, you can also use the root `just` helpers:

```bash
just fmt
just fix -p <crate>
```

Additional documentation:

- [Installing and building](./docs/install.md)
- [Contributing](./docs/contributing.md)

## Notes

- Some repository documentation still describes the original upstream Codex project
- The README, docs structure, release process, and project positioning will continue to evolve for Dopax
- Until an official release process exists, source builds are the primary way to use this repository

## License

This repository currently continues to follow the upstream license model and is distributed under [Apache-2.0](./LICENSE).
