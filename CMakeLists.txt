cmake_minimum_required(VERSION 3.8)
project(bullet)

set(CMAKE_CXX_STANDARD 17)
set(SOURCE_FILES
        main.cpp
        C:/Users/owczy/CLionProjects/glad/output/src/glad.c
        )
add_executable(bullet ${SOURCE_FILES})

add_subdirectory(C:/Users/owczy/CLionProjects/glfw [binary_dir])

include_directories(
        C:/Users/owczy/CLionProjects/glfw/include
        C:/Users/owczy/CLionProjects/glad/output/include
        )

target_link_libraries(bullet glfw ${OPENGL_glu_LIBRARY} ${GLFW_LIBRARIES})