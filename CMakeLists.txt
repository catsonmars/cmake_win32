cmake_minimum_required(VERSION 3.12)

project("CMakeProject1")
add_executable (CMakeProject1 WIN32 "CMakeProject1.cpp" )


if (CMAKE_VERSION VERSION_GREATER 3.12)
  set_property(TARGET CMakeProject1 PROPERTY CXX_STANDARD 20)
   

endif()
