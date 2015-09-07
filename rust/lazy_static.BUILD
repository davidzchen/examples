load("/tools/build_rules/rust/rust", "rust_library", "rust_test")

package(default_visibility = ["//visibility:public"])

rust_library(
    name = "lazy_static",
    srcs = ["src/lib.rs"],
)

rust_test(
    name = "test",
    srcs = ["tests/test.rs"],
    deps = [
        ":lazy_static",
    ],
)
