# This is a static library example
add_library(shape STATIC shape.cc)

# A directory with header files
target_include_directories(shape PUBLIC ${CMAKE_SOURCE_DIR}/includes)

target_compile_options(shape PRIVATE -Wall -Werror)
