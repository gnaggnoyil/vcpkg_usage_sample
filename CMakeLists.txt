cmake_minimum_required(VERSION 3.14 FATAL_ERROR)

if(NOT DEFINED CMAKE_TOOLCHAIN_FILE)
	if(DEFINED ENV{VCPKG_ROOT})
		set(CMAKE_TOOLCHAIN_FILE "$ENV{VCPKG_ROOT}/scripts/buildsystems/vcpkg.cmake")
	endif()
endif()

project(test_proj1)

add_subdirectory(src)