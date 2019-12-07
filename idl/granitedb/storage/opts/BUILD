load("@rules_proto//proto:defs.bzl", "proto_library")
load("@rules_cc//cc:defs.bzl", "cc_proto_library")

#
# The proto targets
#

proto_library(
    name = "update_arithmetic_proto",
    srcs = ["update_arithmetic.proto"],
    visibility = ["//visibility:public"],
)

proto_library(
    name = "update_delete_proto",
    srcs = ["update_delete.proto"],
    visibility = ["//visibility:public"],
)

proto_library(
    name = "update_put_proto",
    srcs = ["update_put.proto"],
    visibility = ["//visibility:public"],
)

proto_library(
    name = "update_script_proto",
    srcs = ["update_script.proto"],
    visibility = ["//visibility:public"],
)

#
# The cc proto targets
#

cc_proto_library(
    name = "update_arithmetic_cc_proto",
    visibility = ["//visibility:public"],
    deps = [":update_arithmetic_proto"],
)

cc_proto_library(
    name = "update_delete_cc_proto",
    visibility = ["//visibility:public"],
    deps = [":update_delete_proto"],
)

cc_proto_library(
    name = "update_put_cc_proto",
    visibility = ["//visibility:public"],
    deps = [":update_put_proto"],
)

cc_proto_library(
    name = "update_script_cc_proto",
    visibility = ["//visibility:public"],
    deps = [":update_script_proto"],
)
