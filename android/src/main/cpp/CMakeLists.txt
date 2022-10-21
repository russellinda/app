cmake_minimum_required(VERSION 3.24.2)

add_subdirectory(curl)
INCLUDE_DIRECTORIES("curl/include")

add_library(
        main
        SHARED
        main.cpp)
target_link_libraries(
        main
        curl)
