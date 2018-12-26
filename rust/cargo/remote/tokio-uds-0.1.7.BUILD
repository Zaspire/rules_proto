"""
cargo-raze crate build file.

DO NOT EDIT! Replaced on runs of cargo-raze
"""

package(default_visibility = [
    # Public for visibility by "@raze__crate__version//" targets.
    #
    # Prefer access through "//rust/cargo", which limits external
    # visibility to explicit Cargo.toml dependencies.
    "//visibility:public",
])

licenses([
    "notice",  # "MIT,Apache-2.0"
])

load(
    "@io_bazel_rules_rust//rust:rust.bzl",
    "rust_binary",
    "rust_library",
    "rust_test",
)

rust_library(
    name = "tokio_uds",
    srcs = glob(["**/*.rs"]),
    crate_features = [
    ],
    crate_root = "src/lib.rs",
    crate_type = "lib",
    rustc_flags = [
        "--cap-lints=allow",
    ],
    version = "0.1.7",
    deps = [
        "@raze__bytes__0_4_11//:bytes",
        "@raze__futures__0_1_25//:futures",
        "@raze__iovec__0_1_2//:iovec",
        "@raze__libc__0_2_45//:libc",
        "@raze__log__0_3_9//:log",
        "@raze__mio__0_6_16//:mio",
        "@raze__mio_uds__0_6_7//:mio_uds",
        "@raze__tokio_core__0_1_17//:tokio_core",
        "@raze__tokio_io__0_1_10//:tokio_io",
    ],
)
