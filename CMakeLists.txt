cmake_minimum_required(VERSION 3.6)

project(fetch_sample)

add_library(fetch
    common.c
    fetch.c
    file.c
    ftp.c
    http.c
)

add_executable(ftc main.cc)
target_link_libraries(ftc fetch)