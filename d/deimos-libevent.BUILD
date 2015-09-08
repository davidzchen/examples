load("/tools/build_defs/d/d", "d_source_library")

package(default_visibility = ["//visibility:public"])

licenses(["notice"])

d_source_library(
    name = "libevent",
    srcs = glob(["deimos/event2/*.d"]),
    linkopts = [
        "-levent",
        "-levent_pthreads",
    ],
    imports = ["."],
)
