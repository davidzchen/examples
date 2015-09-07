load("/tools/build_rules/rust/rust", "rust_library")

package(default_visibility = ["//visibility:public"])

rust_library(
    name = "libc",
    srcs = ["rust/src/liblibc/lib.rs"],
    crate_features = [
        "default",
        "cargo-build"
    ],
)
