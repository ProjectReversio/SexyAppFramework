cmake_minimum_required(VERSION 3.18)

add_subdirectory(SexyAppFramework)

option(BuildDemos "Build Demos" ON)

if (${BuildDemos})
	add_subdirectory(demos)
endif()