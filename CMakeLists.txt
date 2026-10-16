cmake_minimum_required(VERSION 3.21)
project(frame_window_counter CXX)

find_package(Geode REQUIRED)

file(GLOB_RECURSE SRC_FILES src/*.cpp)

geode_target_mod(frame_window_counter
    CPP_FILES
        ${SRC_FILES}
)
