load("@rules_proto//proto:defs.bzl", "proto_library")
load("@rules_cc//cc:defs.bzl", "cc_proto_library")

#
# The proto targets
#

proto_library(
    name = "ensure_proto",
    srcs = ["ensure.proto"],
    visibility = ["//visibility:public"],
    deps = [
        "//idl/common:status_proto",
    ],
)

proto_library(
    name = "read_proto",
    srcs = ["read.proto"],
    visibility = ["//visibility:public"],
)

proto_library(
    name = "sync_proto",
    srcs = ["sync.proto"],
    visibility = ["//visibility:public"],
)

proto_library(
    name = "update_proto",
    srcs = ["update.proto"],
    visibility = ["//visibility:public"],
    deps = [
        ":ensure_proto",
        "//idl/granitedb/storage/opts:update_arithmetic_proto",
        "//idl/granitedb/storage/opts:update_delete_proto",
        "//idl/granitedb/storage/opts:update_put_proto",
        "//idl/granitedb/storage/opts:update_script_proto",
    ],
)

#
# The cc proto targets
#

cc_proto_library(
    name = "ensure_cc_proto",
    visibility = ["//visibility:public"],
    deps = [":ensure_proto"],
)

cc_proto_library(
    name = "read_cc_proto",
    visibility = ["//visibility:public"],
    deps = [":read_proto"],
)

cc_proto_library(
    name = "sync_cc_proto",
    visibility = ["//visibility:public"],
    deps = [":sync_proto"],
)

cc_proto_library(
    name = "update_cc_proto",
    visibility = ["//visibility:public"],
    deps = [":update_proto"],
)
