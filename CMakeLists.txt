cmake_minimum_required(VERSION 3.5.0)
project(6502Emulator VERSION 0.1.0 LANGUAGES C CXX)

#Enable Testing
set(ENABLE_TESTING TRUE)
set(TEST_CPU TRUE)
set(TEST_MEMORY TRUE)
set(TEST_INSTRUCTIONS TRUE)
set(TEST_PROGRAMS TRUE)


include_directories(inc)
add_subdirectory(src)

if(ENABLE_TESTING)
    enable_testing()
    add_subdirectory(test)
endif()

