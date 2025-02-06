cmake_minimum_required(VERSION 3.30)
project(cpp_fps_game)

include(FetchContent)
set(BUILD_SHARED_LIBS OFF)
fetchcontent_declare(SFML GIT_REPOSITORY https://github.com/SFML/SFML.git GIT_TAG 3.0.0)
fetchcontent_makeavailable(SFML)

set(CMAKE_CXX_STANDARD 17)

add_executable(cpp_fps_game src/main.cpp)

target_link_libraries(cpp_fps_game sfml-graphics)