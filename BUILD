cc_library(
  name = 'snappy',
  export_incs = [
    '.',
  ],
  srcs = [
    'snappy.cc',
    'snappy-c.cc',
    'snappy-sinksource.cc',
    'snappy-stubs-internal.cc',
  ],
  warning = 'no'
)

cc_test(
  name = 'snappy_unittest',
  srcs = [
    'snappy_unittest.cc',
    'snappy-test.cc',
  ],
  defs = [
    'HAVE_SYS_MMAN_H',
    'HAVE_SYS_RESOURCE_H',
    'HAVE_SYS_TIME_H',
  ],
  deps = [
    ':snappy',
    '//zlib:zlib',
  ],
  testdata = [
    'testdata'
  ],
  warning = 'no'
)
