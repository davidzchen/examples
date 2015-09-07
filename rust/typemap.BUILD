load("/tools/build_rules/rust/rust", "rust_library")

package(default_visibility = ["//visibility:public"])

rust_library(
    name = "typemap",
    srcs = [
        "src/lib.rs",
        "src/internals.rs",
    ],
    deps = [
        "@unsafe_any//:unsafe_any",
    ],
)
