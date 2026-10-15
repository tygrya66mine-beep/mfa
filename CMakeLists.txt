cmake_minimum_required(VERSION 3.21)
project(macro_analyzer)

find_package(Geode REQUIRED)

geode_target_mod(macro_analyzer
    CPP_FILES
        src/main.cpp
)
