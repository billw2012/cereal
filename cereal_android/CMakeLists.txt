cmake_minimum_required(VERSION 3.5)

file(GLOB_RECURSE header_files ../include/*.h ../include/*.hpp)
 
add_library(cereal STATIC ${header_files})
set_target_properties(cereal PROPERTIES LINKER_LANGUAGE CXX)
