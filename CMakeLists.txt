#######################################
# / CMakeLists.txt
#######################################

cmake_minimum_required (VERSION 2.6) 

project (msgpack-lite) 

enable_testing()

# Add the tests subdirectory
add_subdirectory (tests) 

# install header file
install(FILES ${CMAKE_CURRENT_SOURCE_DIR}/msgpack/msgpack-lite.hpp
        DESTINATION ${CMAKE_INSTALL_PREFIX}/include/msgpack)
