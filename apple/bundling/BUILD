licenses(["notice"])

filegroup(
    name = "dsym_info_plist_template",
    srcs = ["dSYM-Info.plist.template"],
    # Used by the rule implementations, so it needs to be public; but
    # should be considered an implementation detail of the rules and
    # not used by other things.
    visibility = ["//visibility:public"],
)

# Consumed by bazel tests.
filegroup(
    name = "for_bazel_tests",
    testonly = 1,
    srcs = glob(["**"]) + [
        "//apple/bundling/runners:for_bazel_tests",
    ],
    visibility = [
        "//apple:__subpackages__",
    ],
)
