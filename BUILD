load("@bazel_gazelle//:def.bzl", "gazelle")
load("@io_bazel_rules_go//go:def.bzl", "go_library")

# gazelle:prefix github.com/davidsmd/go-ethereum

gazelle(
    name = "gazelle",
    prefix = "github.com/davidsmd/go-ethereum",
)

go_library(
    name = "go_default_library",
    srcs = ["interfaces.go"],
    importpath = "github.com/davidsmd/go-ethereum",
    visibility = ["//visibility:public"],
    deps = [
        "//common:go_default_library",
        "//core/types:go_default_library",
    ],
)
