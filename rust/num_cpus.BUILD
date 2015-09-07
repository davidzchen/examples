load("/tools/build_rules/rust/rust", "rust_library")

package(default_visibility = ["//visibility:public"])

rust_library(
    name = "num_cpus",
    srcs = ["src/lib.rs"],
    deps = [
        "@libc//:libc",
    ],
)
