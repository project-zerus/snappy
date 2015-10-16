cc_library(
  name = 'snappy',
  visibility = ['//visibility:public'],
  includes = [
    '.',
  ],
  srcs = [
    'snappy.cc',
    'snappy-c.cc',
    'snappy-sinksource.cc',
    'snappy-stubs-internal.cc',
  ]
)

cc_binary(
  name = 'snappy_unittest',
  srcs = [
    'snappy_unittest.cc',
    'snappy-test.cc',
  ],
  defines = [
    'HAVE_SYS_MMAN_H',
    'HAVE_SYS_RESOURCE_H',
    'HAVE_SYS_TIME_H',
  ],
  deps = [
    ':snappy',
    '//external:gtest_main',
    '//external:z',
  ],
  data = glob(["testdata/*"]),
)
