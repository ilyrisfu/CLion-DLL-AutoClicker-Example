cmake_minimum_required(VERSION 3.28)
project(AutoClicker)

set(CMAKE_CXX_STANDARD 20)

add_library(AutoClicker SHARED
        dllMain.cpp
        source/me/sleepyfox/autoclicker/ClickUtils.h
        source/me/sleepyfox/autoclicker/Utils.h
)

target_link_libraries(AutoClicker PRIVATE
        winmm
)