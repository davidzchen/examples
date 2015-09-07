load("/tools/build_rules/rust/rust", "rust_library", "rust_binary")

package(default_visibility = ["//visibility:public"])

rust_library(
    name = "plugin",
    srcs = ["src/lib.rs"],
    deps = [
        "@typemap//:typemap",
    ],
)

rust_binary(
    name = "default_types",
    srcs = ["examples/default_types.rs"],
    deps = [
        ":plugin",
        "@typemap//:typemap",
        "@void//:void",
    ],
)
