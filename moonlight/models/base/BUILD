# Description:
# Common logic for all model training.

package(
    default_visibility = ["//moonlight:__subpackages__"],
)

licenses(["notice"])  # Apache 2.0

py_library(
    name = "batches",
    srcs = ["batches.py"],
    srcs_version = "PY2AND3",
    deps = [
        # absl dep
    ],
)

py_test(
    name = "batches_test",
    srcs = ["batches_test.py"],
    srcs_version = "PY2AND3",
    deps = [
        ":batches",
        # absl dep
        # tensorflow dep
    ],
)

py_library(
    name = "glyph_patches",
    srcs = ["glyph_patches.py"],
    srcs_version = "PY2AND3",
    deps = [
        ":batches",
        "//moonlight/protobuf:protobuf_py_pb2",
        # absl dep
        # tensorflow dep
    ],
)

py_test(
    name = "glyph_patches_test",
    srcs = ["glyph_patches_test.py"],
    srcs_version = "PY2AND3",
    deps = [
        ":glyph_patches",
        # numpy dep
        # tensorflow dep
    ],
)
