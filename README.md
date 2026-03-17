# Dopax

Dopax is a fork of [OpenAI Codex](https://github.com/openai/codex), focused on custom product work, workflow experiments, and project-specific extensions built on top of the Codex codebase.

This repository keeps the upstream Codex architecture and core capabilities as its foundation while evolving in its own direction over time.

## What This Project Is

- A Codex-based project built on top of the upstream `openai/codex` repository
- A place to develop custom behavior, integrations, and product ideas
- A fork that is intended to stay aware of upstream changes so it can continue to sync from the official project when needed

## Current Status

This project is still under active development and restructuring.

There are currently **no released packages** for this repository:

- no installable binary releases
- no npm package
- no Homebrew package

For now, the project should be built and run directly from source.

## Relationship To Upstream

- Upstream repository: [`openai/codex`](https://github.com/openai/codex)
- This repository is a maintained fork with project-specific customization
- Some structure, docs, and implementation details still reflect the upstream layout and will be gradually adapted for Dopax

## Local Development

The recommended way to build and run the project is from the `codex-rs` workspace:

```bash
git clone https://github.com/tensorstaff/dopax.git
cd dopax/codex-rs

cargo build
cargo run --bin codex -- "explain this codebase to me"
```

If you are working on the repository regularly, you can also use the root `just` helpers:

```bash
just fmt
just fix -p <crate>
```

Additional documentation:

- [Installing and building](./docs/install.md)
- [Contributing](./docs/contributing.md)

## Notes

- Some repository documentation still describes the original upstream Codex project
- The README, docs structure, release process, and project positioning will continue to be revised for Dopax
- Until an official release process exists, source builds are the primary way to use this repository

## License

This repository currently continues to follow the upstream license model and is distributed under [Apache-2.0](./LICENSE).

