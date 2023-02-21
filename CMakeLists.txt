cmake_minimum_required(VERSION 3.5)

project(NET_L1 LANGUAGES CXX)

set(CMAKE_CXX_STANDARD 17)
set(CMAKE_CXX_STANDARD_REQUIRED ON)

add_executable(NET_L1 main.cpp
    socket.cpp
    socket_wrapper.cpp ${ALLHEADERS})

install(TARGETS NET_L1
    LIBRARY DESTINATION ${CMAKE_INSTALL_LIBDIR})
