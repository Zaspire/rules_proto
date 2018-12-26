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

# Unsupported target "atomic_cell" with type "bench" omitted
# Unsupported target "atomic_cell" with type "test" omitted
# Unsupported target "cache_padded" with type "test" omitted

rust_library(
    name = "crossbeam_utils",
    srcs = glob(["**/*.rs"]),
    crate_features = [
        "default",
        "std",
    ],
    crate_root = "src/lib.rs",
    crate_type = "lib",
    rustc_flags = [
        "--cap-lints=allow",
    ],
    version = "0.6.3",
    deps = [
        "@raze__cfg_if__0_1_6//:cfg_if",
    ],
)

# Unsupported target "parker" with type "test" omitted
# Unsupported target "thread" with type "test" omitted
