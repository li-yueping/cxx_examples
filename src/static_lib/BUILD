load("@rules_cc//cc:defs.bzl", "cc_library")

package(
    default_visibility = ["//visibility:public"], # 对所有包可见
)

cc_library(
    name = "static_lib",                   # 目标名称即库名称
    srcs = glob(["*.cc"]),              # 生成库依赖源文件
    hdrs = glob(["*.h"]),               # 生成库依赖头文件    
    linkstatic = 1 # 只生成静态库
    #visibility = ["//src/main:__pkg__"], # 让当前目标对于工作空间的src/main包可见。默认情况下目标仅仅被当前包可见
    #copts = ["-Isrc/lib"]
)