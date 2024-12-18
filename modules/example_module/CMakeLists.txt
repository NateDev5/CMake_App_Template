add_library(example_module
        src/example.cpp
        include/example.h
)

target_include_directories(example_module PUBLIC ${CMAKE_CURRENT_SOURCE_DIR})