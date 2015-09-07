load("/tools/build_rules/rust/rust", "rust_library")

package(default_visibility = ["//visibility:public"])

rust_library(
    name = "hyper",
    srcs = glob(["src/**/*.rs"]),
    deps = [
        "@cookie//:cookie",
        "@httparse//:httparse",
        "@log//:log",
        "@mime//:mime",
        "@num_cpus//:num_cpus",
        "@openssl//:openssl",
        "@rustc_serialize//:rustc_serialize",
        "@time//:time",
        "@unicase//:unicase",
        "@url//:url",
        "@traitobject//:traitobject",
        "@typeable//:typeable",
    ],
)
