load("//tensorboard/defs:web.bzl", "tf_web_library", "tf_web_test")

package(
    default_testonly = True,
    default_visibility = ["//tensorboard:internal"],
)

licenses(["notice"])  # Apache 2.0

tf_web_test(
    name = "test",
    src = "/tf-color-scale/test/tests.html",
    web_library = ":test_web_library",
)

tf_web_library(
    name = "test_web_library",
    srcs = [
        "colorScaleTests.ts",
        "tests.html",
    ],
    path = "/tf-color-scale/test",
    deps = [
        "//tensorboard/components/tf_color_scale",
        "//tensorboard/components/tf_imports:polymer",
        "//tensorboard/components/tf_imports:web_component_tester",
    ],
)
