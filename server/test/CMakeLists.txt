project(mdb-tests)

add_executable(tests main.cpp)
target_link_libraries(tests PRIVATE messagedb-lib gtest pthread)

add_test(mdb-lib-tests tests)
