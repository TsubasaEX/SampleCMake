cmake_minimum_required(VERSION 3.16.3)
project(testsome)
add_executable(testsome main.cpp)
# target_link_directories(testsome PRIVATE ${CMAKE_SOURCE_DIR}/../../SomeLibDemo/cpp/build)
target_link_libraries(testsome mearlymath)
message(STATUS "start install message")
install(TARGETS testsome DESTINATION bin) # make install -> will install the binary to /usr/local/bin