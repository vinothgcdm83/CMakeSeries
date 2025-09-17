cmake_minimum_required(VERSION 4.0)

project(Rooster)

#The math library
include(src/math/maths.cmake)

# the stats library
include(src/stats/stats.cmake)

add_executable(rooster src/main.cpp)
target_link_libraries(rooster  PUBLIC libstats)
