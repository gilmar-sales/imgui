cmake_minimum_required(VERSION 3.28)

add_library(imgui
    imgui.cpp
    imgui_demo.cpp
    imgui_draw.cpp
    imgui_widgets.cpp
    misc/cpp/imgui_stdlib.cpp
)

add_library(imgui::imgui ALIAS imgui)

target_include_directories(imgui PUBLIC ${CMAKE_CURRENT_SOURCE_DIR})
