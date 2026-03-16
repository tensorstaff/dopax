# Dopax

Agent-native client for computer I/O operations.

## Overview

Dopax is being designed as a focused client for computer I/O operations through an interactive agent interface. The goal is to create a product that feels native to real engineering workflows: multi-step tasks, file edits, terminal execution, project context, long-running sessions, and human-in-the-loop control.

Instead of acting like a simple chat window, Dopax is intended to function as a workspace-aware operator for development tasks. It should help users reason through work, take action inside a project, and keep progress organized across sessions.

## Product Direction

Dopax is being shaped around five core ideas:

- **Agent-native interaction**: the primary interface is built around tasks, turns, tools, and follow-through.
- **Workspace awareness**: actions should be grounded in the local project, not detached from files and runtime state.
- **Controlled autonomy**: the system should be capable of executing work while keeping the user in control of permissions and decisions.
- **Operational clarity**: users should be able to understand what the agent is doing, why it is doing it, and what changed.
- **Extensible foundations**: the client should be able to evolve across models, toolchains, runtimes, and deployment styles.

## Intended Capabilities

The long-term product scope includes the following capability areas:

### 1. Interactive Agent Sessions

- Task-oriented conversational workflows
- Multi-turn reasoning with persistent thread state
- Resume, branch, and revisit previous work
- Structured handling of long-running tasks

### 2. Local Workspace Actions

- Read and edit project files
- Run shell commands in controlled environments
- Inspect logs, outputs, and generated artifacts
- Track file-level changes during a session

### 3. Tool Execution

- Built-in local tools for common development tasks
- External tool connections through a provider-neutral tool layer
- Permission-aware execution with clear user review points
- Support for both synchronous and background workflows

### 4. Project Context Management

- Repository and directory awareness
- Session memory and state continuity
- Structured summaries of ongoing work
- Context reduction and compaction for longer sessions

### 5. User Control and Safety

- Explicit permission boundaries
- Transparent action history
- Interrupt, cancel, and recover flows
- Safe handling of risky or destructive operations

## Experience Principles

Dopax is intended to feel:

- **Fast** enough for daily use
- **Calm** under complex or noisy workflows
- **Readable** when the agent is making decisions
- **Reliable** when files, commands, and session state matter
- **Opinionated** about quality without becoming rigid

The ideal experience is less "chat assistant" and more "operational client for intelligent computer I/O operations."

## Architecture Goals

The product architecture is planned around a few stable layers:

### Client Layer

- Desktop or terminal-facing user experience
- Session navigation, input handling, output rendering
- Permission prompts and user approvals

### Runtime Layer

- Turn processing and task orchestration
- Tool scheduling and execution control
- Context assembly, memory, and state transitions

### Provider Layer

- Model provider abstraction
- Authentication and credential handling
- Request/response normalization
- Streaming and event translation

### Tool Layer

- Local system tools
- External service integrations
- Structured schemas for tool inputs and outputs
- Safety rules and execution policy

## Current Repository Status

This repository is currently in an early foundation stage.

At the moment, it contains:

- Initial brand assets
- Early project framing
- A first pass at visual identity for Dopax

The runtime, client, protocol, and implementation layers described above are product direction, not a published feature-complete release in this repository yet.

## Repository Contents

- `dopax-primary.svg`: primary horizontal logo
- `dopax-mark.svg`: icon-only brand mark
- `README.md`: project overview and direction

## Brand Notes

The current visual system uses:

- A rounded `d`-shaped outer form for a stable and product-led silhouette
- A crossed internal structure that hints at routing, synthesis, and decision flow
- A warm orange-to-amber gradient to avoid generic cold-tech branding
- A deep ink accent for contrast, readability, and trust

Core colors:

- `#F36A42`
- `#FFB13C`
- `#122033`
- `#586676`

## Near-Term Priorities

The next practical milestones are:

1. Define the first runnable client surface
2. Establish core session and tool abstractions
3. Implement a minimal local workflow loop
4. Add authentication and provider integration boundaries
5. Expand repository structure beyond brand assets

## Positioning

Dopax is meant to become a serious client for intelligent computer I/O operations: not only for asking questions, but for planning work, taking action, and staying accountable to the state of a real project.
