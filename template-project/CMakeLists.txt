cmake_minimum_required(VERSION 3.15)

message("Using toolchain file: ${CMAKE_TOOLCHAIN_FILE}")

project(projectname LANGUAGES C ASM)

add_subdirectory(src)
