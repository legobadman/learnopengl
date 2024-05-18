cmake_minimum_required(VERSION 3.13.5)

project(learnopengl)

file(GLOB_RECURSE source CONFIGURE_DEPENDS *.h *.cpp *.c *.fs *.vs)

add_executable(learnopengl ${source})

target_include_directories(learnopengl PRIVATE . include)
target_link_libraries(learnopengl ${CMAKE_CURRENT_SOURCE_DIR}/glfw3.lib)