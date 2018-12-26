sh_test(
    name = "cowsay_test",
    size = "small",
    srcs = ["cowsay_test.sh"],
    data = [
        #TODO(tmc): eliminate these deps
        "@my_packages//cowsay",
    ],
    args = ["$(location @my_packages//cowsay)"],
)
sh_test(
    name = "cowthink_test",
    size = "small",
    srcs = ["cowthink_test.sh"],
    data = [
        "@my_packages//cowsay:cowthink",
    ],
    args = ["$(location @my_packages//cowsay:cowthink)"],
)
