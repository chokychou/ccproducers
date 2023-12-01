package(default_visibility = ["//visibility:public"])

cc_library(
    name = "error",
    hdrs = ["error.h"],
)

cc_library(
    name = "value",
    hdrs = ["value.h"],
)

cc_library(
    name = "input",
    hdrs = ["input.h"],
    deps = [
        ":error",
        ":value",
    ],
)

cc_library(
    name = "output",
    hdrs = ["output.h"],
    deps = [
        ":error",
        ":value",
    ],
)

cc_library(
    name = "node",
    srcs = ["node.cc"],
    hdrs = ["node.h"],
    deps = [
        ":error",
        ":input",
        ":output",
    ],
)

cc_library(
    name = "producer_graph",
    hdrs = ["producer_graph.h"],
    deps = [
        ":error",
        ":input",
        ":node",
        ":output",
    ],
)

cc_test(
    name = "producers_integration_test",
    srcs = ["producers_integration_test.cc"],
    deps = [
        ":output",
        ":producer_graph",
        "//third_party/gtest",
    ],
)
