# Changelog
All notable changes to this project will be documented in this file.

The format is based on [Keep a Changelog](http://keepachangelog.com/en/1.0.0/)
and this project adheres to [Semantic Versioning](http://semver.org/spec/v2.0.0.html).

## [Unreleased]

- Split out of [roblabla/cargo-travis](https://github.com/roblabla/cargo-travis)
  - Includes rename from `cargo-doc-upload` to `cargo-ghp-upload`
  - Call as `cargo ghp-upload [FLAGS] [OPTIONS]`
- No longer links against `cargo`
- CLI changes:
  - New repeatable `-v`/`--verbose` flag for more logging (modulo #1)
  - New `--remove-index` flag to opt-out of maintaining `index.html`
    (It will still be clobbered if an index.html exists in the uploaded folder)
  - New `--directory <upload_directory>` option to upload from directories other than `./target/doc`
- Now can infer much more context from Git if not in Travis-like environment
- Default commit message changed

  [Unreleased]: https://github.com/crate-ci/cargo-ghp-upload/tree/master