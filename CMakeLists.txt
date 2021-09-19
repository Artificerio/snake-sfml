cmake_minimum_required(VERSION 3.17)
set(CXX_STANDARD 17)
set(CMAKE_CXX_STANDARD_REQUIRED ON)

project(snake)

add_executable(project1 main.cpp
	includes/Snake.cpp
	includes/Game.cpp
	includes/World.cpp
	includes/Textbox.cpp
	includes/Window.cpp)
	
target_include_directories(project1 PUBLIC /usr/include/SFML)
target_link_libraries(project1 sfml-system sfml-graphics sfml-window)

