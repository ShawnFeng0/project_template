cmake_minimum_required(VERSION 3.19)
project(project_template)

set(CMAKE_CXX_STANDARD 14)

add_executable(${PROJECT_NAME} src/main.cpp)

add_subdirectory(src/lib)
target_link_libraries(${PROJECT_NAME} PRIVATE library)

add_subdirectory(src/uorb_msg)
target_link_libraries(${PROJECT_NAME} PRIVATE uorb_msg)
