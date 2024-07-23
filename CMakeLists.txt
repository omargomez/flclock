
cmake_minimum_required(VERSION 3.15)
project(Project)
# Uncomment to set custom package path
list(APPEND CMAKE_PREFIX_PATH "/Users/omar.gomez1/.local")
find_package(FLTK CONFIG REQUIRED)
add_executable(flclock WIN32 MACOSX_BUNDLE main.cpp)
target_link_libraries(flclock  PRIVATE fltk::fltk)
