cmake_minimum_required (VERSION 2.6)
project (OPEN_SURF)
# The version number.
set (OPEN_SURF_VERSION_MAJOR 0)
set (OPEN_SURF_VERSION_MINOR 1)

# Set target directories
SET (CMAKE_RUNTIME_OUTPUT_DIRECTORY ${CMAKE_BINARY_DIR}/../bin)
SET (CMAKE_LIBRARY_OUTPUT_DIRECTORY ${CMAKE_BINARY_DIR}/../lib)
SET (CMAKE_ARCHIVE_OUTPUT_DIRECTORY ${CMAKE_BINARY_DIR}/../lib)

# Set directories
include_directories(${OPEN_SURF_SOURCE_DIR}/include)

# Set platform
SET (PLATFORM 64)

#This may need to be updated or Linux/Windows
SET (CMAKE_LIBRARY_PATH ${CMAKE_LIBRARY_PATH} /opt/local/lib)

find_package(OpenCV REQUIRED)

#include_directories(${OPENGL_INCLUDE_DIRS} ${GLUT_INCLUDE_DIRS})
#link_directories (${OPENGL_LIBRARY_DIRS} ${GLUT_LIBRARY_DIRS})

#include_directories("${OPEN_SURF_SOURCE_DIR}/sift")

add_subdirectory(src)