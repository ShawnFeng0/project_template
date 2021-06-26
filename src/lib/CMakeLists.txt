project(library)

add_library(${PROJECT_NAME} INTERFACE)

add_subdirectory(ulog)
target_link_libraries(${PROJECT_NAME} INTERFACE ulog)

add_subdirectory(uorb)
target_link_libraries(${PROJECT_NAME} INTERFACE uorb)

add_subdirectory(vrb)
target_link_libraries(${PROJECT_NAME} INTERFACE vrb)

add_subdirectory(ucfg)
target_link_libraries(${PROJECT_NAME} INTERFACE ucfg)
