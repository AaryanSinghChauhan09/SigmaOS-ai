# SigmaOS AI

AI and machine learning experiments organized as a Rust library. The crate exposes `ai` and `ml` modules, including agent and orchestration code, local inference interfaces, quantization helpers, tensor data structures, and training primitives.

This repository is an evolving collection of integrations and prototypes. A module's presence does not imply that it connects to a live model provider, executes hardware acceleration, or is suitable for production use. Review each implementation and its dependencies before relying on it.

## Build

The crate uses a sibling path dependency on [`SigmaOS-kernel`](../SigmaOS-kernel), so build it from the SigmaOS checkout with:

```sh
cargo check --manifest-path SigmaOS-ai/Cargo.toml --lib
```

## Layout

- `src/ai/` contains AI-facing modules such as agents, orchestration, local LLM interfaces, and quantization.
- `src/ml/` contains inference, training, and data workspace primitives.
- `src/lib.rs` is the crate entry point.

## License

GPL-3.0-or-later. See [`Cargo.toml`](Cargo.toml).
