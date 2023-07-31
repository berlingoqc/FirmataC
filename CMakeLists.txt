# CMakeList.txt : Pour le librairie libardrone
cmake_minimum_required (VERSION 3.8)

project (firmatac VERSION 0.0.1 LANGUAGES CXX)

include_directories(${CMAKE_CURRENT_SOURCE_DIR}/includes)

# Crée ma target de la librairie
add_library (firmatac STATIC src/firmata.cpp src/serial.cpp src/servo.cpp)
