cmake_minimum_required(VERSION 3.10)
project(SudokuSFML)

set(CMAKE_CXX_STANDARD 17)

find_package(SFML 2.5 COMPONENTS graphics window system REQUIRED)

add_executable(sudoku src/main.cpp)

target_link_libraries(sudoku sfml-graphics sfml-window sfml-system)
