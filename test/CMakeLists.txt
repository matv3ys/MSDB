add_executable(tests tests.cpp)
target_link_libraries(tests PRIVATE msdb::libmsdb Catch2::Catch2WithMain)