load("/tools/build_rules/rust/rust", "rust_library")

package(default_visibility = ["//visibility:public"])

rust_library(
    name = "unsafe_any",
    srcs = ["src/lib.rs"],
    deps = [
        "@traitobject//:traitobject",
    ],
)
