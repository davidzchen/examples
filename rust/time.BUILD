load("/tools/build_rules/rust/rust", "rust_library")

package(default_visibility = ["//visibility:public"])

cc_library(
    name = "time_helpers",
    srcs = ["src/time_helpers.c"],
    copts = [
        "-ffunction-sections",
        "-fdata-sections",
        "-fPIC",
    ],
)

rust_library(
    name = "time",
    srcs = ["src/lib.rs"],
    deps = [
        ":time_helpers",
        "@libc//:libc",
    ],
)
