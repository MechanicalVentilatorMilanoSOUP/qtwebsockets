# Generated from qmlwebsocketserver.pro.

cmake_minimum_required(VERSION 3.14)
project(qmlwebsocketserver LANGUAGES CXX)

set(CMAKE_INCLUDE_CURRENT_DIR ON)

set(CMAKE_AUTOMOC ON)
set(CMAKE_AUTORCC ON)
set(CMAKE_AUTOUIC ON)

set(INSTALL_EXAMPLEDIR "examples/websockets/qmlwebsocketserver")

find_package(Qt6 COMPONENTS Core)
find_package(Qt6 COMPONENTS Gui)
find_package(Qt6 COMPONENTS Quick)
find_package(Qt6 COMPONENTS WebSockets)

add_executable(qmlwebsocketserver
    main.cpp
)
target_link_libraries(qmlwebsocketserver PUBLIC
    Qt::Core
    Qt::Gui
    Qt::Quick
    Qt::WebSockets
)


# Resources:
set(data_resource_files
    "qml/qmlwebsocketserver/main.qml"
)

qt6_add_resources(qmlwebsocketserver "data"
    PREFIX
        "/"
    FILES
        ${data_resource_files}
)

install(TARGETS qmlwebsocketserver
    RUNTIME DESTINATION "${INSTALL_EXAMPLEDIR}"
    BUNDLE DESTINATION "${INSTALL_EXAMPLEDIR}"
    LIBRARY DESTINATION "${INSTALL_EXAMPLEDIR}"
)
