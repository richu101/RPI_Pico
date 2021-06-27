# version

cmake_minimum_required(VERSION 3.16)

include(pico_sdk_import.cmake)

project(Blink_LED_project)
pico_sdk_init()
add_executable(Blink blink.c)


target_link_libraries(Blink pico_stdlib)

pico_add_extra_outputs(Blink)
