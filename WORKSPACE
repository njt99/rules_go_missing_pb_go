git_repository(
  name = "io_bazel_rules_go",
  remote = "https://github.com/bazelbuild/rules_go",
  commit = "76acdc5c4ab7321fa6f26936f4efa42a2a2c0b01",
)
load("@io_bazel_rules_go//go:def.bzl", "go_rules_dependencies", "go_register_toolchains", "go_repository")
go_rules_dependencies()
go_register_toolchains()
load("@io_bazel_rules_go//proto:def.bzl", "proto_register_toolchains")
proto_register_toolchains()

go_repository(
    name = "com_github_chrislusf_gleam",
    importpath = "github.com/chrislusf/gleam",
    commit = "f87a51bfb042028bf903e19fbbce308b828f2790",
)
