# Bazel run example

    # This is executable Markdown that's tested on CI.
    set -o errexit -o nounset -o xtrace
    alias ~~~=":<<'~~~sh'";:<<'~~~sh'

## Try it out

Run the sh_binary target with `aspect run`.
It should locate the data.json file from the runfiles.

~~~sh
output="$(aspect run //:bin)"

# Verify that it produces the expected output
echo "${output}" | grep -q "Hello, world!" || {
    echo >&2 "Wanted output containing 'Hello, world!' but got '${output}'"
    exit 1
}
~~~

Run multiple programs:

~~~sh
aspect multi_run -- //:bin //:program2
~~~

