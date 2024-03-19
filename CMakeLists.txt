cmake_minimum_required(VERSION 3.2)

project(test)

set(CMAKE_CXX_STANDARD 11)

add_subdirectory(Bcrypt.cpp)

add_executable(test main.cpp)
target_link_libraries(test PRIVATE bcrypt)
