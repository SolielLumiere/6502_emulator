set(CPU_LIBRARY cpulib CACHE INTERNAL "")
include_directories(${PROJECT_SOURCE_DIR}/inc/CPU)
add_library(${CPU_LIBRARY} ICPU.cpp CPU.cpp Addressing.cpp)