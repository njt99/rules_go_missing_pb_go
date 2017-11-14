load("@io_bazel_rules_go//go:def.bzl", "gazelle", "go_binary", "go_library")

gazelle(
    name = "gazelle",
    prefix = "github.com/njt99/rules_go_missing_pb_go",
)

go_library(
    name = "go_default_library",
    srcs = ["demo.go"],
    importpath = "github.com/njt99/rules_go_missing_pb_go",
    visibility = ["//visibility:private"],
    deps = ["@com_github_chrislusf_gleam//pb:go_default_library"],
)

go_binary(
    name = "rules_go_missing_pb_go",
    importpath = "github.com/njt99/rules_go_missing_pb_go",
    library = ":go_default_library",
    visibility = ["//visibility:public"],
)
