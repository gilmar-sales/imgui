project(ImGui)

add_library(imgui
        imgui.cpp
        imgui_demo.cpp
        imgui_draw.cpp
        imgui_tables.cpp
        imgui_widgets.cpp
        )

target_include_directories(imgui INTERFACE
        PUBLIC
        $<INSTALL_INTERFACE:/>
        $<BUILD_INTERFACE:${CMAKE_CURRENT_SOURCE_DIR}/>
        ${CMAKE_CURRENT_SOURCE_DIR}/
        )