COPTS = ["-Wall",
         "-Werror",
         "-I include",]

LINKOPTS = ["-lyaml"]

cc_binary(
  name="numerical",
  copts = COPTS,
  linkopts = LINKOPTS,
  srcs = ["numerical/main.c"],
  deps = [
    "//src:libcyaml",
  ]
)

