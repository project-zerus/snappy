cc_library(
  name = 'snappy',
  srcs = [
    'snappy.cc',
    'snappy-c.cc',
    'snappy-sinksource.cc',
    'snappy-stubs-internal.cc'
  ],
  export_incs = '.',
  warning = 'no',
)

cc_test(
  name = 'snappy_unittest',
  defs = [
    'HAVE_SYS_MMAN_H',
    'HAVE_SYS_RESOURCE_H',
    'HAVE_SYS_TIME_H',
  ],
  srcs = [
    'snappy_unittest.cc',
    'snappy-test.cc',
  ],
  deps = [
    ':snappy',
    '//zlib:zlib',
  ],
  testdata = [
    'testdata',
  ],
  warning = 'no',
)
