
sh_test(
    name = "cowsay_test",
    size = "small",
    srcs = ["cowsay_test.sh"],
    data = [
        # TODO(tmc): figure out how to remove these dependencies
        "@homebrew_core//:allfiles",
        "@brew//:binaries",
        "@brew_packages//:cowsay",
    ],
)
sh_test(
    name = "cowthink_test",
    size = "small",
    srcs = ["cowthink_test.sh"],
    data = ["@brew_packages//:cowthink"],
)
