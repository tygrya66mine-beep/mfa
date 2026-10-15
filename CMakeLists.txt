cmake_minimum_required(VERSION 3.25)
project(macro_analyzer CXX)

find_package(Geode REQUIRED)

geode_target_mod(macro_analyzer
    CPP_FILES
        src/main.cpp
)
