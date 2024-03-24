cmake_minimum_required(VERSION 3.19)

set(CMAKE_CXX_STANDARD 20)
set(CMAKE_CXX_STANDARD_REQUIRED ON)
set(CMAKE_MODULE_PATH ${CMAKE_CURRENT_SOURCE_DIR}/cmake/module)

project(http CXX)

set(HTTPLIB_REQUIRE_OPENSSL ON)

add_subdirectory(openssl-cmake)
add_subdirectory(cpp-httplib)
add_subdirectory(examples)

