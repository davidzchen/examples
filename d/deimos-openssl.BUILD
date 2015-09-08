load("/tools/build_defs/d/d", "d_source_library")

package(default_visibility = ["//visibility:public"])

licenses(["notice"])

d_source_library(
    name = "openssl",
    srcs = glob(["deimos/openssl/*.d"]),
    linkopts = [
        "-lssl",
        "-lcrypto",
    ],
    imports = ["."],
)
