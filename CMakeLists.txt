cmake_minimum_required(VERSION 2.8.11)
project(dcadec)

set(CMAKE_C_FLAGS "${CMAKE_C_FLAGS} -std=gnu99 -D_FILE_OFFSET_BITS=64 -Wall -Wextra -O3 -ffast-math -g -MMD")

add_library(dcadec STATIC
  libdcadec/bitstream.c
  libdcadec/core_decoder.c
  libdcadec/dca_context.c
  libdcadec/dmix_tables.c
  libdcadec/exss_parser.c
  libdcadec/idct_fixed.c
  libdcadec/idct_float.c
  libdcadec/interpolator.c
  libdcadec/interpolator_fixed.c
  libdcadec/interpolator_float.c
  libdcadec/lbr_decoder.c
  libdcadec/ta.c
  libdcadec/xll_decoder.c
  libdcadec/dca_frame.c
  libdcadec/dca_stream.c
  libdcadec/dca_waveout.c
  )
