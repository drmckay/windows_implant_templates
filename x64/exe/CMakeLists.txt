# CMakeList.txt : CMake project for exe, include source and define
# project specific logic here.
#
cmake_minimum_required (VERSION 3.8)

project(meterpreter_x64_asm ASM_MASM)
# Add source to this project's executable.
add_executable (meterpreter_x64_asm "meterpreter_x64_windows.asm")



target_compile_options(meterpreter_x64_asm 
	PUBLIC
	/link /subsystem:windows /defaultlib:kernel32.lib /entry:main
)