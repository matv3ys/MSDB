add_library(libmsdb libmsdb.cpp)
add_library(msdb::libmsdb ALIAS libmsdb)

set_target_properties(
        libmsdb
        PROPERTIES OUTPUT_NAME msdb
)

target_compile_features(libmsdb PUBLIC cxx_std_17)
target_include_directories(
        libmsdb
        PRIVATE include
        PUBLIC ${CMAKE_SOURCE_DIR}/include
)