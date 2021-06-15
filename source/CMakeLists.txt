cmake_minimum_required(VERSION 3.18)

option(WideStrings "Wide Strings" ON)
if (${WideStrings})
	add_compile_definitions(_USE_WIDE_STRING)
endif()

add_subdirectory(SexyAppFramework)

option(BuildDemos "Build Demos" ON)

if (${BuildDemos})
	add_subdirectory(demos)
endif()