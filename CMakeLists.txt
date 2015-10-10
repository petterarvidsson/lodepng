cmake_minimum_required(VERSION 2.8 FATAL_ERROR)
project(lodepng)

file (GLOB Sources
  "lodepng.cpp"
  "lodepng.h"
  )

add_library(lodepng ${Sources})
install (TARGETS lodepng DESTINATION lib)
install (FILES lodepng.h DESTINATION include)
