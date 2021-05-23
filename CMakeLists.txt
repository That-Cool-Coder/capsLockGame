cmake_minimum_required(VERSION 3.10)

project(capsLockGame VERSION 1.0)

set(CMAKE_CXX_STANDARD 17)
set(CMAKE_CXX_STANDARD_REQUIRED True)

file(GLOB SOURCES "src/*.cpp")
add_executable(capsLockGame ${SOURCES})

target_include_directories(capsLockGame PUBLIC
    "${PROJECT_BINARY_DIR}"
)