cmake_minimum_required(VERSION 3.14)
project(MCE-Tests VERSION 1.0 LANGUAGES CXX)

set(INCLUDE_PATH include)
include_directories(${INCLUDE_PATH})

set(SRC_PATH src)
set(
    TEST_SRC_FILES

    ${SRC_PATH}/main.cpp
    ${SRC_PATH}/world.cpp
)

add_executable(mce-tests ${TEST_SRC_FILES})

target_link_libraries(mce-tests PRIVATE mce)
