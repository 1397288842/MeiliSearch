# GitHub actions workflow for MeiliDB

> **Note:**
> - The repository is currently compiling with Rust Nighlty, we aim to compile on Rust stable as soon as possible.
> - We do not use [cache](https://github.com/actions/cache) yet but we could use it to speed up CI

## Workflow

-  On each pull request, we are triggering `cargo test`.
- On each commit on master, we are building the latest docker image.
- On each tag, we are building the tagged docker image and the binaries for Debian & CentOS
