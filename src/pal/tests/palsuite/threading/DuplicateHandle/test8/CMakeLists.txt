cmake_minimum_required(VERSION 2.8.12.2)

set(CMAKE_INCLUDE_CURRENT_DIR ON)

set(SOURCES
  test8.c
)

add_executable(paltest_duplicatehandle_test8
  ${SOURCES}
)

add_dependencies(paltest_duplicatehandle_test8 CoreClrPal)

target_link_libraries(paltest_duplicatehandle_test8
  pthread
  m
  CoreClrPal
)
