load("@rules_proto//proto:defs.bzl", "proto_library")
load("@rules_cc//cc:defs.bzl", "cc_proto_library")

#
# The proto targets
#

proto_library(
    name = "status_proto",
    srcs = ["status.proto"],
    visibility = ["//visibility:public"],
)

#
# The cc proto targets
#

cc_proto_library(
    name = "status_cc_proto",
    visibility = ["//visibility:public"],
    deps = [":status_proto"],
)
