cmake_minimum_required(VERSION 4.2)
project(kraken)

find_package(OpenGL REQUIRED)
find_package(glad CONFIG REQUIRED)
find_package(glfw3 CONFIG REQUIRED)

add_executable(kraken game.cpp)

target_link_libraries(kraken
    PRIVATE
    OpenGL::GL
    glad::glad
    glfw
)
