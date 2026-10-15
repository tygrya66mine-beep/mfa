cmake_minimum_required(VERSION 3.21)
project(macro_analyzer CXX)

if(NOT Geode_FOUND)
    if(DEFINED ENV{GEODE_SDK})
        set(Geode_DIR "$ENV{GEODE_SDK}")
    endif()
endif()

find_package(Geode REQUIRED)

geode_target_mod(macro_analyzer
    CPP_FILES
        src/main.cpp
)
