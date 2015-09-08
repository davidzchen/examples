load("/tools/build_defs/d/d", "d_library")

package(default_visibility = ["//visibility:public"])

licenses(["notice"])

d_library(
    name = "vibe-d",
    srcs = glob(
        ["source/vibe/**/*.d"],
        exclude = ["source/vibe/appmain.d"],
    ),
    deps = [
        "@deimos-libevent//:libevent",
        "@deimos-openssl//:openssl",
    ],
    imports = ["source"],
    versions = ["VibeLibeventDriver"],
)

d_library(
    name = "vibe-d_main",
    srcs = ["source/vibe/appmain.d"],
    deps = [":vibe-d"],
    imports = ["source"],
    versions = ["VibeDefaultMain"],
)
