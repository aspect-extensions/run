load("@rules_shell//shell:sh_binary.bzl", "sh_binary")

sh_binary(
    name = "bin",
    srcs = ["bin.sh"],
    data = ["data.json"],
    deps = ["@bazel_tools//tools/bash/runfiles"],
    tags = ["default_run_mux"],
)

sh_binary(
    name = "program2",
    srcs = ["program2.sh"],
    tags = ["default_run_mux"],
)
