package(default_visibility = ["//visibility:public"])

licenses(["notice"])

load(
    "@io_bazel_rules_go//go:def.bzl",
    "go_library",
    "go_test",
)

go_library(
    name = "go_default_library",
    srcs = ["ovirt.go"],
    tags = ["automanaged"],
    deps = [
        "//pkg/api/v1:go_default_library",
        "//pkg/cloudprovider:go_default_library",
        "//pkg/types:go_default_library",
        "//vendor:gopkg.in/gcfg.v1",
    ],
)

go_test(
    name = "go_default_test",
    srcs = ["ovirt_test.go"],
    library = ":go_default_library",
    tags = ["automanaged"],
    deps = ["//pkg/cloudprovider:go_default_library"],
)
