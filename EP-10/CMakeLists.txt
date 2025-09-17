cmake_minimum_required(VERSION 4.0)

project(Rooster)

#The math library
add_subdirectory(src/maths)

# the stats library
add_subdirectory(src/stats)

add_executable(rooster src/main.cpp)
target_link_libraries(rooster  PUBLIC libstats)
