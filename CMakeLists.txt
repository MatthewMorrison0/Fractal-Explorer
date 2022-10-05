cmake_minimum_required(VERSION 3.9)
project(Fractal_Explorer)
set(CMAKE_CXX_STANDARD 11)

add_subdirectory(lib/glfw-master)
add_subdirectory(lib/glew-cmake-master)
add_subdirectory("lib/Fractal_Explorer")

target_include_directories(${PROJECT_NAME} PUBLIC ${CMAKE_CURRENT_SOURCE_DIR}/lib/glfw-master/include)
target_include_directories(${PROJECT_NAME} PUBLIC ${CMAKE_CURRENT_SOURCE_DIR}/lib/glew-cmake-master/include)
