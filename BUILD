package(default_visibility = ["//visibility:public"])

load(
  "@io_tweag_rules_haskell//haskell:haskell.bzl",
  "haskell_binary",
  "haskell_library",
  "haskell_toolchain",
)

haskell_toolchain(
  name = "ghc",
  version = "8.2.2",
  tools = "@ghc//:bin",
)

haskell_binary(
  name = "subtyping",
  srcs = glob(['*.hs']),
    prebuilt_dependencies = [
        "base",
        "parsec",
        "containers",
        "mtl",
        "haskeline"
    ],
)
