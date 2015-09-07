load("/tools/build_rules/rust/rust", "rust_library", "rust_test")

package(default_visibility = ["//visibility:public"])

rust_library(
    name = "cookie",
    srcs = [
        "src/lib.rs",
        "src/jar.rs",
    ],
    deps = [
        "@url//:url",
        "@time//:time",
        "@rustc_serialize//:rustc_serialize",
        "@openssl//:openssl",
    ],
    crate_features = [
        "default",
        "rustc-serialize",
        "openssl",
    ],
)

rust_test(
    name = "lib",
    srcs = [
        "src/lib.rs",
        "src/jar.rs",
    ],
    deps = [
        "@url//:url",
        "@time//:time",
        "@rustc_serialize//:rustc_serialize",
        "@openssl//:openssl",
    ],
    crate_features = [
        "default",
        "rustc-serialize",
        "openssl",
    ],
)
