workspace(name = "com_google_fhir_examples")

load("@bazel_tools//tools/build_defs/repo:http.bzl", "http_archive")
http_archive(
    name = "com_google_fhir",
    sha256 = "79c860b95bccc577997718ddd8ac2bf9a72475e2f1d9cf5dac86004a7e22a3ce",
    strip_prefix = "fhir-f042f19de529ff42cc15a06f2cfcade502144037",
    urls = [
        "https://github.com/google/fhir/archive/f042f19de529ff42cc15a06f2cfcade502144037.zip",
    ],
)

load("@com_google_fhir//bazel:dependencies.bzl", "fhirproto_dependencies")
fhirproto_dependencies()

load("@com_google_fhir//bazel:workspace.bzl", "fhirproto_workspace")
fhirproto_workspace()

load("@com_google_fhir//bazel:go_dependencies.bzl", "fhir_go_dependencies")
fhir_go_dependencies()
