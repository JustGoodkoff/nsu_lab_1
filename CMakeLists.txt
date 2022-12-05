cmake_minimum_required(VERSION 3.20)
set(This Test)

set(Sources Test.cpp)

add_executable(${This} ${Sources})
target_link_libraries(${This} PUBLIC
        gtest_main
        nsu_oop)
add_test(
        NAME ${This}
        COMMAND ${This}
)