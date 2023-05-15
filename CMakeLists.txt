cmake_minimum_required(VERSION 3.11)
project(
    your_project
    VERSION 0.1.0
    DESCRIPTION "This is your project. Change on your own."
    LANGUAGES CXX
)

set(CMAKE_CXX_STANDARD 17)

add_subdirectory(app)
add_subdirectory(lib)
add_subdirectory(tests)

set(CPACK_PROJECT_NAME ${PROJECT_NAME})
set(CPACK_PROJECT_VERSION ${PROJECT_VERSION})
include(CPack)
