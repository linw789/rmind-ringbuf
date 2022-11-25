cmake_minimum_required(VERSION 3.21)

project(rmind_ringbuf LANGUAGES C)

add_library(rmind_ringbuf STATIC
    inc/rmind/ringbuf.h
    src/ringbuf.c
)

target_include_directories(rmind_ringbuf PUBLIC inc)

set_target_properties(rmind_ringbuf PROPERTIES
    C_STANDARD 11
)
