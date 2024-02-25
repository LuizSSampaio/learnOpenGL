cmake_minimum_required(VERSION 3.28)
project(learnOpenGL)

set(CMAKE_CXX_STANDARD 20)

find_package(glad CONFIG REQUIRED)
find_package(glfw3 CONFIG REQUIRED)

add_executable(learnOpenGL main.cpp)

target_link_libraries(learnOpenGL PRIVATE glad::glad glfw)
