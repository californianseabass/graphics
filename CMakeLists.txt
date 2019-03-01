cmake_minimum_required(VERSION 3.2)
project(graphicsdemo)

find_package(GLUT REQUIRED)
find_package(OpenGL REQUIRED)
include_directories( ${OPENGL_INCLUDE_DIRS}  ${GLUT_INCLUDE_DIRS} )

#set(CMAKE_CXX_FLAGS "-g -Wall")
add_executable(main main.cpp)
target_link_libraries(main ${OPENGL_LIBRARIES} ${GLUT_LIBRARY} )
