# CMakeList.txt : Top-level CMake project file, do global configuration
# and include sub-projects here.
#
cmake_minimum_required (VERSION 3.8)

project ("Hello-GiNaC")

# Add GiNaC
set(CLN_DIR ${CMAKE_CURRENT_SOURCE_DIR}/lib/GiNaC/cmake/modules)
add_subdirectory(${CMAKE_CURRENT_SOURCE_DIR}/lib/GiNaC)

# Include sub-projects.
add_subdirectory ("Hello-GiNaC")
