load("/tools/build_rules/rust/rust", "rust_library")

package(default_visibility = ["//visibility:public"])

rust_library(
    name = "conduit_mime_types",
    srcs = ["src/lib.rs"],
    data = ["data/mime.json"],
    deps = [
        "@rustc_serialize//:rustc_serialize",
    ],
)
