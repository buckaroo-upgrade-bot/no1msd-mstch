load('//:subdir_glob.bzl', 'subdir_glob')
load('//:buckaroo_macros.bzl', 'buckaroo_deps')

cxx_library(
  name = 'mstch',
  header_namespace = '',
  exported_headers = subdir_glob([
    ('include', '**/*.hpp'),
  ]),
  headers = subdir_glob([
    ('src', '**/*.hpp'),
  ]),
  srcs = glob([
    'src/**/*.cpp',
  ]),
  licenses = [
    'LICENSE',
  ],
  deps = buckaroo_deps(),
  visibility = [
    'PUBLIC'
  ],
)
