cmake_minimum_required(VERSION 3.0.0)

project(spsstereo VERSION 1.0.0)

set(CPACK_PROJECT_NAME ${PROJECT_NAME})
set(CPACK_PROJECT_VERSION ${PROJECT_VERSION})

if(NOT CMAKE_BUILD_TYPE)
  set(CMAKE_BUILD_TYPE Release)
endif()

add_executable(spsstereo spsstereo_main.cpp SPSStereo.cpp SGMStereo.cpp)

target_compile_options(spsstereo PRIVATE "-msse4.2")

target_link_libraries(spsstereo png)
