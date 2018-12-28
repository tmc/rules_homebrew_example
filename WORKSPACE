load("@bazel_tools//tools/build_defs/repo:git.bzl", "git_repository", "new_git_repository")
git_repository(
    name = "com_github_tmc_rules_homebrew",
    remote = "https://github.com/tmc/rules_homebrew.git",
    branch = "master",
)
#local_repository( name = "com_github_tmc_rules_homebrew", path = "../rules_homebrew")

load("@com_github_tmc_rules_homebrew//rules:def.bzl", "homebrew_repository")

homebrew_repository(
    name = "my_packages",
    packages = [
        "cowsay",
        "jq",
        "cloc",
    ],
    #verbose = True,
)

