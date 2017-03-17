prebuilt_cxx_library(
  name = 'egl',
  header_only = True,
  header_namespace = '',
  exported_headers = subdir_glob([
    ('api', 'EGL/*.h'),
    ('api', 'KHR/*.h'),
  ]),
  visibility = [
    'PUBLIC',
  ],
)

cxx_library(
  name = 'test',
  srcs = [
    'api/egltest.c',
  ],
  deps = [
    ':egl',
  ],
)
