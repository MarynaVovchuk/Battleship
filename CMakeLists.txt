cmake_minimum_required(VERSION 3.20)
project(battleship)

set(CMAKE_CXX_STANDARD 20)
set(CMAKE_AUTOMOC ON)
set(CMAKE_AUTORCC ON)
set(CMAKE_AUTOUIC ON)

find_package(Qt6 COMPONENTS
		Core
		Gui
		Widgets
                Network
		Sql
		Test
		REQUIRED)

add_subdirectory(3rdparty)
enable_testing()
add_subdirectory(src)
