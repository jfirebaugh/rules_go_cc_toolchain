```
$ BAZEL_DO_NOT_DETECT_CPP_TOOLCHAIN=1 bazel build --@io_bazel_rules_go//go/config:pure //:main     
ERROR: /private/var/tmp/_bazel_john/1a1601b430d3853275c40a0975b48db0/external/io_bazel_rules_go/BUILD.bazel:86:17: While resolving toolchains for target @io_bazel_rules_go//:cgo_context_data: No matching toolchains found for types @bazel_tools//tools/cpp:toolchain_type.
To debug, rerun with --toolchain_resolution_debug='@bazel_tools//tools/cpp:toolchain_type'
If platforms or toolchains are a new concept for you, we'd encourage reading https://bazel.build/concepts/platforms-intro.
ERROR: Analysis of target '//:main' failed; build aborted: 
INFO: Elapsed time: 11.215s
INFO: 0 processes.
FAILED: Build did NOT complete successfully (45 packages loaded, 2276 targets configured)
```
