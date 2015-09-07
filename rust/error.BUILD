load("/tools/build_rules/rust/rust", "rust_library", "rust_binary")

package(default_visibility = ["//visibility:public"])

rust_library(
    name = "error",
    srcs = ["src/lib.rs"],
    deps = [
        "@traitobject//:traitobject",
        "@typeable//:typeable",
    ],
)

rust_binary(
    name = "downcast",
    srcs = ["examples/downcast.rs"],
    deps = [
        ":error",
    ],
)
