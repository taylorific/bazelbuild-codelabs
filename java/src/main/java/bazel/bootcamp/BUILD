java_binary(
    name = "HelloBazelBootcamp",
    srcs = ["HelloBazelBootcamp.java"],
)

java_library(
    name = "JavaLoggingClientLibrary",
    srcs = ["JavaLoggingClientLibrary.java"],
    deps = [
        "//proto/logger:logger_java_proto",
        "//proto/logger:logger_java_grpc",
        "@io_grpc_grpc_java//core",
        "@io_grpc_grpc_java//netty",
    ]
)

java_binary(
    name = "JavaLoggingClient",
    srcs = ["JavaLoggingClient.java"],
    deps = [":JavaLoggingClientLibrary"],
    visibility = ["//visibility:public"]
)
