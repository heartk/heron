java_test(
    name = "CommunicatorTest",
    srcs = glob(["**/CommunicatorTest.java"]),
    deps = [
        "//heron/common/src/java:common-java",
        "@bazel_tools//third_party:junit4",
    ],
    size = "small",
)

java_test(
    name = "SysUtilsTest",
    srcs = glob(["**/SysUtilsTest.java"]),
    deps = [
        "//heron/common/src/java:common-java",
        "@bazel_tools//third_party:junit4",
    ],
    size = "small",
)

java_test(
    name = "WakeableLooperTest",
    srcs = glob(["**/WakeableLooperTest.java"]),
    deps = [
        "//heron/common/src/java:common-java",
        "@bazel_tools//third_party:junit4",
    ],
    size = "small",
)

java_test(
    name = "FileUtilsTest",
    srcs = glob(["**/FileUtilsTest.java"]),
    deps = [
        "//heron/common/src/java:common-java",
        "//3rdparty/java:powermock",
        "@bazel_tools//third_party:mockito",
        "@bazel_tools//third_party:junit4",
    ],
    size = "small",
)

java_test(
    name = "EchoTest",
    srcs = glob(["**/EchoTest.java"]),
    deps = [
        "//heron/common/src/java:common-java",
        "//heron/proto:proto_networktests_java",
        "@protobuf-java//jar",
        "@bazel_tools//third_party:junit4",
    ],
    size = "small",
)

java_test(
    name = "HeronServerTest",
    srcs = glob(["**/HeronServerTest.java"]),
    deps = [
        "//heron/common/src/java:common-java",
        "//heron/proto:proto_networktests_java",
        "@protobuf-java//jar",
        "@bazel_tools//third_party:junit4",
    ],
    size = "small",
)

java_library(
    name = "config-test-java",
    srcs = glob(["**/config/Constants.java"]),
)

java_test(
    name = "ConfigReaderTest",
    srcs = glob(["**/config/ConfigReaderTest.java"]),
    deps = [
        ":config-test-java",
        "//heron/common/src/java:config-java",
        "@bazel_tools//third_party:junit4",
    ],
    data = glob(["**/config/testdata/**/*.yaml"]),
    size = "small",
)

java_test(
    name = "ClusterConfigReaderTest",
    srcs = glob(["**/config/ClusterConfigReaderTest.java"]),
    deps = [
        ":config-test-java",
        "//heron/common/src/java:config-java",
        "@bazel_tools//third_party:junit4",
    ],
    data = glob(["**/config/testdata/**/*.yaml"]),
    size = "small",
)

java_test(
    name = "SystemConfigTest",
    srcs = glob(["**/config/SystemConfigTest.java"]),
    deps = [
        ":config-test-java",
        "//heron/common/src/java:config-java",
        "@bazel_tools//third_party:junit4",
    ],
    data = glob(["**/config/testdata/sysconfig.yaml"]),
    size = "small",
)
