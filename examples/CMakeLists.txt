add_library(common STATIC common.cpp)
target_include_directories(common PUBLIC ${CMAKE_CURRENT_SOURCE_DIR})
target_compile_features(common PUBLIC cxx_std_11)

add_subdirectory(main)
add_subdirectory(server)
add_subdirectory(quantize)