cmake_minimum_required(VERSION 3.16)
project(SFML_Project_template)

set(CMAKE_CXX_STANDARD 11)

add_executable(SFML_Project_template main.cpp)

add_subdirectory(include/SFML)

target_link_libraries(SFML_Project_template
        PUBLIC
        sfml-graphics sfml-window sfml-system sfml-network sfml-audio)

target_include_directories(SFML_Project_template PRIVATE)