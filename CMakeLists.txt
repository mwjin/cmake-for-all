cmake_minimum_required(VERSION 3.11)
project(
    your_project
    VERSION 0.1.0
    DESCRIPTION "This is your project. Change on your own."
    LANGUAGES CXX
)

include(CTest)
enable_testing()

add_executable(your_project main.cc)

set(CPACK_PROJECT_NAME ${PROJECT_NAME})
set(CPACK_PROJECT_VERSION ${PROJECT_VERSION})
include(CPack)
