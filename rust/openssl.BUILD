load("/tools/build_rules/rust/rust", "rust_library")

package(default_visibility = ["//visibility:public"])

cc_library(
    name = "old_openssl_shim",
    srcs = ["openssl-sys/src/old_openssl_shim.c"],
    linkopts = [
        "-lssl",
        "-lcrypto",
    ],
    copts = [
        "-Wdeprecated-declarations",
        "-ffunction-sections",
        "-fdata-sections",
        "-fPIC",
    ],
)

rust_library(
    name = "openssl_sys",
    srcs = glob(["openssl-sys/src/*.rs"]),
    deps = [
        ":old_openssl_shim",
        "@libc//:libc",
    ],
    rustc_flags = [
        "-l dylib=crypto",
        "-l dylib=ssl",
    ],
)

rust_library(
    name = "openssl",
    srcs = glob(["openssl/src/**/*.rs"]),
    deps = [
        ":openssl_sys",
        "@bitflags//:bitflags",
        "@lazy_static//:lazy_static",
        "@libc//:libc",
    ],
)
