cmake_minimum_required(VERSION 3.20)

add_library(template_lib STATIC
  ${CMAKE_CURRENT_SOURCE_DIR}/template_lib.c    
)

set_target_properties(template_lib PROPERTIES 
  OUTPUT_NAME "template_lib"
  PREFIX ""
)

target_include_directories(template_lib PUBLIC ${CMAKE_CURRENT_SOURCE_DIR})