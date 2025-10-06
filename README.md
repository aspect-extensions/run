A replacement for the 'bazel run' command.

Why?

- 'bazel run' has inconsistent behavior about the working directory, which is often set to `$(bazel info execution root)`. See https://github.com/bazelbuild/bazel/issues/3325
- Add support for watch mode
- Ability to run multiple binaries
