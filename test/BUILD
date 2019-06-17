COPTS = ["-Werror",
         "-I include"]

LINKOPTS = ["-lyaml"]

cc_library(
  name = "test_headers",
  hdrs = ["units/ttest.h"]
)

cc_binary(
    name = "test",
    copts = COPTS,
    linkopts = LINKOPTS,
    srcs = glob(["units/*.c"]),
    deps = [
      ":test_headers",
      "//include:cyaml",
      "//src:libcyaml"
    ]
)
