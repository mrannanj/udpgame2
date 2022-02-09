cmake_minimum_required(VERSION 3.18)
project(udpgame2)

set(CMAKE_CXX_STANDARD 14)
set(CMAKE_AUTOMOC ON)
set(CMAKE_AUTORCC ON)
set(CMAKE_AUTOUIC ON)


find_package(Qt5 COMPONENTS
        Core
        Gui
        Widgets
        REQUIRED)

add_executable(udpgame2 main.cpp)
target_link_libraries(udpgame2
        Qt5::Core
        Qt5::Gui
        Qt5::Widgets
        )

