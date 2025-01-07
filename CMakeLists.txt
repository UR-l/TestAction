cmake_minimum_required(VERSION 3.10.0)

project(TestAction C CXX)

add_definitions(-std=c++17)

file(GLOB PROJECT_SRC ${CMAKE_SOURCE_DIR}/include/*.h ${CMAKE_SOURCE_DIR}/src/*.cpp)
set(SRC_FILES ${PROJECT_SRC})

add_executable(${PROJECT_NAME} ${SRC_FILES})

#add_library(${PROJECT_NAME} SHARED ${SRC_FILES})

target_link_libraries(${PROJECT_NAME})


