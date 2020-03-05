# CMakeList.txt : CMake project for exe, include source and define
# project specific logic here.
#
cmake_minimum_required (VERSION 3.8)

project(meterpreter_x86_asm ASM)

#set(CMAKE_SYSTEM_NAME WIN32)
set(CMAKE_SYSTEM_PROCESSOR x86)

set(CMAKE_ARCH x86)
set(CMAKE_ASM_COMPILER_FLAGS "")
set(CMAKE_BUILD_TYPE "Debug")

add_executable(meterpreter_x86_asm "meterpreter_template.s")

#set_target_properties(meterpreter_x86_asm PROPERTIES LINKER_LANGUAGE ASM)
set_target_properties(meterpreter_x86_asm PROPERTIES CMAKE_SYSTEM_PROCESSOR x86)


# TODO: Add tests and install targets if needed.