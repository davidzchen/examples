load("/tools/build_rules/rust/rust", "rust_library", "rust_test")

package(default_visibility = ["//visibility:public"])

rust_library(
    name = "log",
    srcs = [
        "src/lib.rs",
        "src/macros.rs",
    ],
    deps = [
        "@libc//:libc",
    ],
)

rust_test(
    name = "filters",
    srcs = ["tests/filters.rs"],
    deps = [
        ":log",
    ],
)
