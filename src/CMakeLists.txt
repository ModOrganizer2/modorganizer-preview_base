cmake_minimum_required(VERSION 3.16)

add_library(preview_base SHARED)
mo2_configure_plugin(preview_base WARNINGS OFF)
mo2_install_target(preview_base)
