# Copyright 2018 Google LLC
#
# Licensed under the Apache License, Version 2.0 (the "License");
# you may not use this file except in compliance with the License.
# You may obtain a copy of the License at
#
#      http://www.apache.org/licenses/LICENSE-2.0
#
# Unless required by applicable law or agreed to in writing, software
# distributed under the License is distributed on an "AS IS" BASIS,
# WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
# See the License for the specific language governing permissions and
# limitations under the License.

workspace(name = "hashtable_benchmarks")

# abseil
http_archive(
    name = "absl",
    strip_prefix = "abseil-cpp-master",
    urls = ["https://github.com/abseil/abseil-cpp/archive/master.zip"],
)

# Google benchmark.
http_archive(
    name = "gbench",
    strip_prefix = "benchmark-master",
    urls = ["https://github.com/google/benchmark/archive/master.zip"],
)

# Google dense_hash_set
new_http_archive(
    name = "google_sparsehash",
    build_file = "BUILD.sparsehash",
    strip_prefix = "sparsehash-master",
    urls = ["https://github.com/google/sparsehash/archive/master.zip"],
)

http_archive(
    name = "com_github_gflags_gflags",
    strip_prefix = "gflags-master",
    urls = ["https://github.com/gflags/gflags/archive/master.zip"],
)
http_archive(
    name = "com_github_google_glog",
    strip_prefix = "glog-master",
    urls = ["https://github.com/google/glog/archive/master.zip"],
)
new_http_archive(
    name = "com_github_google_double_conversion",
    build_file = "BUILD.double_conversion",
    strip_prefix = "double-conversion-master",
    urls = ["https://github.com/google/double-conversion/archive/master.zip"],
)

# Facebook folly
new_http_archive(
    name = "facebook_folly",
    build_file = "BUILD.folly",
    strip_prefix = "folly-master",
    urls = ["https://github.com/facebook/folly/archive/master.zip"],
)

http_archive(
    name = "com_github_nelhage_rules_boost",
    strip_prefix = "rules_boost-master",
    urls = ["https://github.com/nelhage/rules_boost/archive/master.zip"],
)

load("@com_github_nelhage_rules_boost//:boost/boost.bzl", "boost_deps")

boost_deps()
