cmake_minimum_required( VERSION 3.10 )

project(procxx
        VERSION 0.0.1
        DESCRIPTION "A simple process management library for C++ on UNIX platforms.")

add_library(procxx INTERFACE)
target_include_directories(procxx INTERFACE include/)


option(BUILD_EXAMPLE "Build example" OFF)

if(BUILD_EXAMPLE)
add_subdirectory(example)
endif()
