set(PROJECT_NAME uWebSockets)
project(${PROJECT_NAME} VERSION 0.14.7 LANGUAGES CXX)

set (CMAKE_CXX_STANDARD 14)
include_directories(${PROJECT_NAME} src)

add_library(
	${PROJECT_NAME}
	src/Extensions.cpp
	src/Group.cpp
	src/Networking.cpp
	src/Hub.cpp
	src/Node.cpp
	src/WebSocket.cpp
	src/HTTPSocket.cpp
	src/Socket.cpp
	src/Epoll.cpp
)
