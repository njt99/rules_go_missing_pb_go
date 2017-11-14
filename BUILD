load("@io_bazel_rules_go//go:def.bzl", "gazelle", "go_binary", "go_library")

gazelle(
    name = "gazelle",
    prefix = "github.com/ipvive/challenges",
)

go_library(
    name = "go_default_library",
    srcs = ["demo.go"],
    importpath = "github.com/ipvive/challenges",
    visibility = ["//visibility:private"],
    deps = ["@com_github_chrislusf_gleam//pb:go_default_library"],
)

go_binary(
    name = "challenges",
    importpath = "github.com/ipvive/challenges",
    library = ":go_default_library",
    visibility = ["//visibility:public"],
)
