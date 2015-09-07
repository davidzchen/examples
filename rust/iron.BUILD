load("/tools/build_rules/rust/rust", "rust_library", "rust_binary")

package(default_visibility = ["//visibility:public"])

rust_library(
    name = "iron",
    srcs = glob(["src/**/*.rs"]),
    deps = [
        "@conduit_mime_types//:conduit_mime_types",
        "@error//:error",
        "@hyper//:hyper",
        "@lazy_static//:lazy_static",
        "@log//:log",
        "@modifier//:modifier",
        "@num_cpus//:num_cpus",
        "@plugin//:plugin",
        "@typemap//:typemap",
        "@url//:url",
    ],
)

# Build rules for examples
rust_binary(
    name = "around",
    srcs = ["examples/around.rs"],
    deps = [
        ":iron",
        "@time//:time",
    ],
)

rust_binary(
    name = "404",
    srcs = ["examples/404.rs"],
    deps = [":iron"],
)

rust_binary(
    name = "content_type",
    srcs = ["examples/content_type.rs"],
    deps = [":iron"],
)

rust_binary(
    name = "error",
    srcs = ["examples/error.rs"],
    deps = [
        ":iron",
        "@time//:time",
    ],
)

rust_binary(
    name = "hello",
    srcs = ["examples/hello.rs"],
    deps = [":iron"],
)

rust_binary(
    name = "redirect",
    srcs = ["examples/redirect.rs"],
    deps = [":iron"],
)

rust_binary(
    name = "time",
    srcs = ["examples/time.rs"],
    deps = [
        ":iron",
        "@time//:time",
    ],
)

