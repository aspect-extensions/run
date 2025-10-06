load("@rules_shell//shell:sh_binary.bzl", "sh_binary")

sh_binary(
    name = "bin",
    srcs = ["bin.sh"],
    data = ["data.json"],
    deps = ["@bazel_tools//tools/bash/runfiles"],
)
