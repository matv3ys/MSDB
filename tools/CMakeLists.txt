add_executable(msdb msdb.cpp)
target_link_libraries(msdb PRIVATE msdb::libmsdb PkgConfig::libedit)