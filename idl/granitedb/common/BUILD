load("@rules_proto//proto:defs.bzl", "proto_library")
load("@rules_cc//cc:defs.bzl", "cc_proto_library")

#
# The proto targets
#

proto_library(
    name = "code_proto",
    srcs = ["code.proto"],
    visibility = ["//visibility:public"],
    deps = [
        "//idl/common:status_proto",
    ],
)

#
# The cc proto targets
#

cc_proto_library(
    name = "code_cc_proto",
    visibility = ["//visibility:public"],
    deps = [":code_proto"],
)
