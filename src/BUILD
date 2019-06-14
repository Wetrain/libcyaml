COPTS = ["-Wall",
         "-Werror",
         "-DVERSION_MAJOR=0",
         "-DVERSION_MINOR=1",
         "-DVERSION_PATCH=0",
         "-DVERSION_DEVEL=1"]

cc_library(
  name = "data",
  copts = COPTS,
  hdrs = ["data.h"],
  deps = [
    ":util",
  ],
)

cc_library(
  name = "free",
  copts = COPTS,
  srcs = ["free.c"],
  deps = [
    ":data",
    ":mem",
  ],
)

cc_library(
  name = "load",
  copts = COPTS,
  srcs = ["load.c"],
  deps = [
    ":data",
    ":mem",
  ],
)

cc_library(
  name = "save",
  copts = COPTS,
  srcs = ["save.c"],
  deps = [
    ":data",
    ":mem",
  ],
)

cc_library(
  name = "mem",
  copts = COPTS,
  srcs = ["mem.c"],
  hdrs = ["mem.h"]
)

cc_library(
  name = "utf8",
  copts = COPTS,
  srcs = ["utf8.c"],
  hdrs = ["utf8.h"]
)

cc_library(
  name = "util",
  copts = COPTS,
  srcs = ["util.c"],
  hdrs = ["util.h"],
  deps = [
    ":utf8",
  ],
)

cc_library(
  name = "libcyaml",
  copts = COPTS,
  deps = [
    ":free",
    ":load",
    ":mem",
    ":save",
    ":utf8",
    ":util",
  ],
  visibility = ["//visibility:public"],
)
