cmake_minimum_required(VERSION 3.10)

project(WinVimTiler LANGUAGES CXX)

set(CMAKE_CXX_STANDARD 17)
set(CMAKE_CXX_STANDARD_REQUIRED ON)

add_executable(WinVimTiler WIN32 main.cpp)

# Link against necessary Windows libraries
target_link_libraries(WinVimTiler PRIVATE user32 gdi32) 