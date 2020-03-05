# CMakeList.txt : Top-level CMake project file, do global configuration
# and include sub-projects here.
#
cmake_minimum_required (VERSION 3.8)

project ("windows_implant_templates")

enable_language(C CXX ASM)

# Include sub-projects.
add_subdirectory ("x64")
add_subdirectory ("x86")
