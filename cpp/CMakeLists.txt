cmake_minimum_required(VERSION 3.16)
set(CMAKE_VERBOSE_MAKEFILE ON)
project(HtmlConverter VERSION 1.0
        DESCRIPTION "see readme."
        LANGUAGES CXX)

set(CMAKE_CXX_STANDARD 11)

# uncomment these lines to enable coverage measurements using gcov
#set(CMAKE_CXX_FLAGS "--coverage")

enable_testing()
add_subdirectory(src)
add_subdirectory(test-catch2)
add_subdirectory(test-doctest)
add_subdirectory(test-gtest)

