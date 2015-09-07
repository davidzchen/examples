load("/tools/build_rules/rust/rust", "rust_library", "rust_test")

package(default_visibility = ["//visibility:public"])

rust_library(
    name = "mime",
    srcs = ["src/lib.rs"],
    deps = [
        "@log//:log",
    ],
)

rust_test(
    name = "lib",
    srcs = ["src/lib.rs"],
    deps = [
        "@log//:log",
    ],
)
