# `cargo-cache` GitHub Action

[![GitHub Action](https://img.shields.io/github/actions/workflow/status/raviqqe/cargo-cache/test.yaml?branch=main&style=flat-square)](https://github.com/raviqqe/cargo-cache/actions)
[![License](https://img.shields.io/github/license/raviqqe/cargo-cache.svg?style=flat-square)](UNLICENSE)

> [!Warning]
> Currently, this action works only with Rust on a nightly channel!
> Although you can use this action with a stable channel, it might lead to unbounded cache sizes.

GitHub Action to save and restore Rust build cache in `target` and `~/.cargo` directories

## Current limitations

- Only the nightly channel is supported currently for [cache cleaning](https://blog.rust-lang.org/2023/12/11/cargo-cache-cleaning.html).
- `target` directories can lead to unbounded sizes even with the nightly channel.
- The action **always** saves build cache.
  - For more information see [#4](https://github.com/raviqqe/cargo-cache/issues/4).
- It doesn't support custom `.cargo/config.toml` files.

## References

- [`swatinem/rust-cache`](https://github.com/swatinem/rust-cache) is a good alternative if saving a big cache is not acceptable for your projects.
- [`actions/cache`](https://github.com/actions/cache/blob/main/examples.md)

## License

[The Unlicense](UNLICENSE)
