cmake_minimum_required(VERSION 3.16)

find_package(mo2-cmake CONFIG REQUIRED)
find_package(mo2-uibase CONFIG REQUIRED)

add_library(preview_base SHARED previewbase.cpp previewbase.h)
mo2_configure_plugin(preview_base NO_SOURCES WARNINGS 4)
target_link_libraries(preview_base PRIVATE mo2::uibase)
mo2_install_plugin(preview_base)
