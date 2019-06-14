load("@bazel_tools//tools/build_defs/repo:git.bzl", "new_git_repository")

new_git_repository(
    name = "com_yaml_libyaml",
    remote = "https://github.com/yaml/libyaml.git",
    tag = "dist-0.2.2",
    build_file_content = """
cc_library(
    name = "libyaml",
    srcs = glob(["src/*.cpp"]),
    hdrs =glob(["src/*.h"]),
    visibility = ["//visibility:public"]
 )
""",
)

