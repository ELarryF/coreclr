cmake_minimum_required(VERSION 2.8.12.2)

set(CMAKE_INCLUDE_CURRENT_DIR ON)

set(SOURCES
  test9.cpp
)

add_executable(paltest_vprintf_test9
  ${SOURCES}
)

add_dependencies(paltest_vprintf_test9 coreclrpal)

target_link_libraries(paltest_vprintf_test9
  ${COMMON_TEST_LIBRARIES}
)
