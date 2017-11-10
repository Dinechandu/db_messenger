cmake_minimum_required (VERSION 3.0)
project (daemon)

find_package(Threads REQUIRED)

set (CMAKE_CXX_FLAGS "-fPIC -Wall -std=c++11")

include_directories(${clog_SOURCE_DIR} ${Node_SOURCE_DIR})

add_executable(daemon db_messengerd.cpp)
target_link_libraries(daemon Node)
target_link_libraries(daemon clog)

