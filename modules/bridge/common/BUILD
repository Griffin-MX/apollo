load("//tools:cpplint.bzl", "cpplint")

package(default_visibility = ["//visibility:public"])

cc_library(
    name = "bridge_buffer",
    srcs = [
        "bridge_buffer.cc",
    ],
    hdrs = [
        "bridge_buffer.h",
    ],
)

cc_library(
    name = "bridge_gflags",
    srcs = [
        "bridge_gflags.cc",
    ],
    hdrs = [
        "bridge_gflags.h",
    ],
)

cc_library(
    name = "util",
    srcs = [
        "util.cc",
    ],
    hdrs = [
        "util.h",
    ],
    deps = [
        ":bridge_buffer",
    ],
)

cc_library(
    name = "macro",
    hdrs = [
        "macro.h",
    ],
)

cc_library(
    name = "bridge_header",
    srcs = [
        "bridge_header.cc",
    ],
    hdrs = [
        "bridge_header.h",
        "bridge_header_item.h",
    ],
)

cc_test(
    name = "bridge_buffer_test",
    size = "small",
    srcs = [
        "bridge_buffer_test.cc",
    ],
    deps = [
        ":bridge_buffer",
        "@gtest//:main",
    ],
)

cpplint()
