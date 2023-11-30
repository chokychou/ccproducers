workspace(name = "ccproducers")
load("@bazel_tools//tools/build_defs/repo:http.bzl", "http_archive")


# GoogleTest/GoogleMock framework. Used by most unit-tests.
#       https://github.com/google/googletest
http_archive(
  name = "com_google_googletest",  # 2023-08-02T16:45:10Z
  sha256 = "c4f675500e09da97fd5a2b9c3fdadf48de858a036db565d52e6835c96eeea147",
  strip_prefix = "googletest-843976e4f582ccb76cf87e0f128585324335779b",
  # Keep this URL in sync with ABSL_GOOGLETEST_COMMIT in ci/cmake_common.sh.
  urls = ["https://github.com/google/googletest/archive/843976e4f582ccb76cf87e0f128585324335779b.zip"],
)
