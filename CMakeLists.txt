
cmake_minimum_required(VERSION 3.21)

project(OmniNet VERSION 1.0.0 LANGUAGES CXX)

set(CMAKE_CXX_STANDARD 17)
set(CMAKE_CXX_STANDARD_REQUIRED ON)
set(CMAKE_CXX_EXTENSIONS OFF)

set(CMAKE_AUTOMOC ON)
set(CMAKE_AUTOUIC ON)
set(CMAKE_AUTORCC ON)

find_package(Qt6 6.10 REQUIRED COMPONENTS Widgets Network)

qt_standard_project_setup()

qt_add_executable(OmniNet
    src/main.cpp

    src/routerdiscovery.cpp
    include/routerdiscovery.h

    src/devicediscovery.cpp
    include/devicediscovery.h

    src/authenticationdetector.cpp
    include/authenticationdetector.h

    src/routercredentialwidget.cpp
    include/routercredentialwidget.h

    resources.qrc
)

target_include_directories(OmniNet PRIVATE
    "${CMAKE_CURRENT_SOURCE_DIR}/include"
)

target_link_libraries(OmniNet PRIVATE
    Qt6::Widgets
    Qt6::Network
    iphlpapi
    ws2_32
)
