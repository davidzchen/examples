load("/tools/build_rules/rust/rust", "rust_library")

package(default_visibility = ["//visibility:public"])

rust_library(
    name = "url",
    srcs = glob(["src/*.rs"]),
    deps = [
        "@rustc_serialize//:rustc_serialize",
        "@rust-std-candidates//:matches",
    ],
)
