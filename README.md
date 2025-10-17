A replacement for the 'bazel run' command. and stuff

Why?

- 'bazel run' has inconsistent behavior about the working directory, which is often set to `$(bazel info execution root)`. See https://github.com/bazelbuild/bazel/issues/3325
  - No one wants to write `--run_under="cd $PWD &&"`
- Add support for watch mode
- Ability to run multiple binaries

## multi_run task

[![asciicast](https://asciinema.org/a/NjHTT8Ta67O2rfTc8f4QXW2yB.svg)](https://asciinema.org/a/NjHTT8Ta67O2rfTc8f4QXW2yB)
