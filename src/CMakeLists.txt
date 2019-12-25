find_package(range-v3 0.9.1 EXACT CONFIG REQUIRED)
add_executable(test_proj1 main.cpp)
target_link_libraries(test_proj1 range-v3)