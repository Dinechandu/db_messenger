cmake_minimum_required (VERSION 3.0)
project (client)

find_package(Threads REQUIRED)

set (CMAKE_CXX_FLAGS "-fPIC -Wall -std=c++11")

include_directories(${clog_SOURCE_DIR} ${Node_SOURCE_DIR})

add_executable(client db_messenger.cpp)
target_link_libraries(client Node)
target_link_libraries(client clog)

