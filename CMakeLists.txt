cmake_minimum_required(VERSION 3.9)
project(db_messenger)

add_subdirectory(${PROJECT_SOURCE_DIR}/clog ${PROJECT_SOURCE_DIR}/clog/build)
add_subdirectory(${PROJECT_SOURCE_DIR}/Node ${PROJECT_SOURCE_DIR}/Node/build)

add_subdirectory(${PROJECT_SOURCE_DIR}/client ${PROJECT_SOURCE_DIR}/client/build)
add_subdirectory(${PROJECT_SOURCE_DIR}/daemon ${PROJECT_SOURCE_DIR}/daemon/build)
