cmake_minimum_required(VERSION 3.16)
project(BIA VERSION 0.1)

set(CMAKE_CXX_STANDARD 17)
set(CMAKE_CXX_STANDARD_REQUIRED ON)

find_package(QT NAMES Qt6 Qt5 REQUIRED COMPONENTS Widgets Pdf Gui)

add_executable(bia main.cpp)
target_link_libraries(bia Qt6::Widgets Qt6:Pdf Qt6::Gui)
