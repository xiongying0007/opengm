if(BUILD_EXAMPLES)
   add_subdirectory(examples)
endif()

add_subdirectory(external)
add_subdirectory(interfaces)
add_subdirectory(converter)

message( "${CMAKE_CURRENT_SOURCE_DIR}/sandbox/CMakeLists.txt" )
if(EXISTS "${CMAKE_CURRENT_SOURCE_DIR}/sandbox/CMakeLists.txt")
  add_subdirectory(sandbox)
endif()
