# CMakeList.txt : Pour le librairie libardrone
cmake_minimum_required (VERSION 3.8)

project (firmatac VERSION 0.0.1 LANGUAGES C)

include_directories(${CMAKE_CURRENT_SOURCE_DIR}/includes)

set ( SRC src/firmata.c src/serial.c src/servo.c )

# Crée ma target de la librairie
add_library (firmatac STATIC ${SRC})