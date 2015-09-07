Building Rust with Bazel
========================

This workspace contains example BUILD files for building Rust projects using
Bazel.

This project contains BUILD files for the Rust web framework
[Iron](http://ironframework.io/) and all the Rust crates that Iron depends on.

To build Iron:

```bash
bazel build @iron//:iron
```
