cmake_minimum_required(VERSION 3.19)
project(OPENGL)

set(CMAKE_CXX_STANDARD 14)
include_directories(./include)
link_directories(./lib)
add_executable(${PROJECT_NAME} main.cpp src/glad.c )
target_link_libraries(${PROJECT_NAME}
        "glfw3"
        "openGL32")