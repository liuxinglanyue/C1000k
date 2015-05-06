cmake_minimum_required(VERSION 3.1)
project(C1000k)

set(CMAKE_CXX_FLAGS "${CMAKE_CXX_FLAGS} -std=c++11")

set(SOURCE_FILES server/main.cc)
add_executable(C1000k ${SOURCE_FILES} server/network.h server/socket_util.h server/socket_util.cc server/timers.h server/timers.cc server/network.cc server/worker.cc server/main_event.h server/main_event.cc server/client.cc server/listenfd.cc server/main.cc client/http_client.h client/http_client.cc client/main_event.h client/main_event.cc client/network.h client/network.cpp client/socket_util.h client/socket_util.cc client/timers.h client/timers.cc client/client.cpp client/main.cc client/worker.cpp)