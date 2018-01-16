cmake_minimum_required(VERSION 3.9)

set(CMAKE_CXX_STANDARD 14)
set(CMAKE_CXX_STANDARD)

# create project
project(part_c)

find_package(glfw3 REQUIRED)
find_package(GLEW REQUIRED)

set (SRCS
    simple.cpp
  )
set (HEADERS

  )

add_executable(${CMAKE_PROJECT_NAME} ${SRCS} ${HEADERS})
target_link_libraries(${CMAKE_PROJECT_NAME} glfw ${GLEW_LIBRARIES})

if (APPLE)
  target_link_libraries(${CMAKE_PROJECT_NAME} "-framework OpenGL")
endif()
