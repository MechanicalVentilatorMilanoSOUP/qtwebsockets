# Generated from qmlwebsockets.pro.

#####################################################################
## qmlwebsockets Plugin:
#####################################################################

qt_add_qml_module(qmlwebsockets
    URI "QtWebSockets"
    VERSION "1.0" #special case
    CLASSNAME QtWebSocketsDeclarativeModule
    SKIP_TYPE_REGISTRATION
    SOURCES
        qmlwebsockets_plugin.cpp qmlwebsockets_plugin.h
        qqmlwebsocket.cpp qqmlwebsocket.h
        qqmlwebsocketserver.cpp qqmlwebsocketserver.h
    PUBLIC_LIBRARIES
        Qt::CorePrivate
        Qt::QmlPrivate
        Qt::WebSockets
)

#### Keys ignored in scope 1:.:.:qmlwebsockets.pro:<TRUE>:
# IMPORT_VERSION = "1.$$QT_MINOR_VERSION"
# OTHER_FILES = "qmldir"
# TARGETPATH = "QtWebSockets"
