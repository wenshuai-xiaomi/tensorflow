package(
    default_visibility = [
        # tensorflow/core:lib effectively exposes all targets under tensorflow/core/lib/**
        "//tensorflow/core:__pkg__",
    ],
    licenses = ["notice"],  # Apache 2.0
)

# Todo(bmzhao): Remaining targets to add are: all tests.

cc_library(
    name = "histogram",
    srcs = ["histogram.cc"],
    hdrs = ["histogram.h"],
    deps = [
        "//tensorflow/core/framework:summary_proto_cc",
        "//tensorflow/core/lib/gtl:array_slice",
        "//tensorflow/core/platform:logging",
        "//tensorflow/core/platform:macros",
        "//tensorflow/core/platform:mutex",
        "//tensorflow/core/platform:thread_annotations",
        "//tensorflow/core/platform:types",
    ],
    alwayslink = True,
)

filegroup(
    name = "legacy_lib_histogram_all_headers",
    srcs = [
        "histogram.h",
    ],
    visibility = ["//tensorflow/core:__pkg__"],
)

filegroup(
    name = "legacy_lib_histogram_all_srcs",
    srcs = [
        "histogram.cc",
    ],
    visibility = ["//tensorflow/core:__pkg__"],
)

filegroup(
    name = "legacy_lib_histogram_all_tests",
    srcs = [
        "histogram_test.cc",
    ],
    visibility = ["//tensorflow/core:__pkg__"],
)
