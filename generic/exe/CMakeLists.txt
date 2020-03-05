# CMakeList.txt : CMake project for exe, include source and define
# project specific logic here.
#
cmake_minimum_required (VERSION 3.8)

# Add source to this project's executable.
add_executable (generic_cpp_exe "exe.cpp" "exe.h")
add_executable (generic_c_meterpreter "meterpreter_template.c")

# TODO: Add tests and install targets if needed.
