load(
    "//bazel:envoy_build_system.bzl",
    "envoy_cc_library",
    "envoy_package",
)

licenses(["notice"])  # Apache 2

envoy_package()

envoy_cc_library(
    name = "buffer_interface",
    hdrs = ["buffer.h"],
    external_deps = [
        "abseil_inlined_vector",
    ],
    deps = [
        "//envoy/api:os_sys_calls_interface",
        "//envoy/common:exception_lib",
        "//envoy/http:stream_reset_handler_interface",
        "//source/common/common:assert_lib",
        "//source/common/common:byte_order_lib",
        "//source/common/common:utility_lib",
    ],
)
