#
# Internal library : libev
#
include(ExternalProject)
ExternalProject_Add(
  libev
  SOURCE_DIR ${CMAKE_CURRENT_SOURCE_DIR}/libev
  CONFIGURE_COMMAND ${CMAKE_CURRENT_SOURCE_DIR}/libev/configure --prefix=${CMAKE_CURRENT_SOURCE_DIR}/libev
  PREFIX ${CMAKE_CURRENT_SOURCE_DIR}/libev
  BUILD_COMMAND make
  BUILD_IN_SOURCE 1
)

#
# Main executable
#
add_executable(sirveillance main.cpp)
