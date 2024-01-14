# `cargo-cache` GitHub Action

[![GitHub Action](https://img.shields.io/github/actions/workflow/status/raviqqe/cargo-cache/test.yaml?branch=main&style=flat-square)](https://github.com/raviqqe/cargo-cache/actions)
[![License](https://img.shields.io/github/license/raviqqe/cargo-cache.svg?style=flat-square)](UNLICENSE)

> [!Warning]
> Currently, this action works only with Rust on a nightly channel.

GitHub Action to save and restore Rust build cache in `target` and `~/.cargo` directories

## Current limitations

- Only the nightly channel is supported for [cache cleaning](https://blog.rust-lang.org/2023/12/11/cargo-cache-cleaning.html).
- The action **always** saves build cache.
  - For more information see [#4](https://github.com/raviqqe/cargo-cache/issues/4).
- It doesn't support custom `.cargo/config.toml` files.

## References

- [`actions/cache`](https://github.com/actions/cache/blob/main/examples.md)

## License

[The Unlicense](UNLICENSE)
