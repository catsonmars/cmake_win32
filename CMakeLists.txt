# CMakeList.txt : CMake project for CMakeProject1, include source and define
# project specific logic here.
#

# Add source to this project's executable.
add_executable (CMakeProject1 "CMakeProject1.cpp" )

if (CMAKE_VERSION VERSION_GREATER 3.12)
  set_property(TARGET CMakeProject1 PROPERTY CXX_STANDARD 20)
  add_executable(CMakeProject1 WIN32 CMakeProject1.cpp)
  set_property(DIRECTORY ${CMAKE_CURRENT_SOURCE_DIR} PROPERTY VS_STARTUP_PROJECT CMakeProject1)

endif()

# TODO: Add tests and install targets if needed.
