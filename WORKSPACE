workspace(name = "bootcamp")

load("@bazel_tools//tools/build_defs/repo:http.bzl", "http_archive")

# grpc dependencies
rules_grpc_commit = "a4299eb6bed3c2f2497f583d0c4620c9f31ec455"
rules_grpc_java_sha = "62b0dc1403321e716fc550349011cab008ae158cb4ebb1931644a68f45567387"

http_archive(
    name = "io_grpc_grpc_java",
    urls = [
        "https://github.com/grpc/grpc-java/archive/%s.zip" % rules_grpc_commit,
    ],
    sha256 = rules_grpc_java_sha,
    strip_prefix = "grpc-java-%s" % rules_grpc_commit,
)

load("@io_grpc_grpc_java//:repositories.bzl", "grpc_java_repositories")

grpc_java_repositories()
