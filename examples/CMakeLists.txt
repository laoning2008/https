set(CMAKE_CXX_STANDARD 20)
set(CMAKE_CXX_STANDARD_REQUIRED ON)
set(CMAKE_POLICY_DEFAULT_CMP0077 NEW)
set_property(GLOBAL PROPERTY USE_FOLDERS ON)

project(examples CXX)

add_executable(http_example ${CMAKE_CURRENT_SOURCE_DIR}/main.cpp)
target_link_libraries(http_example PRIVATE httplib)
