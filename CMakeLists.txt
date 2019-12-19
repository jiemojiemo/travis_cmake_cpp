cmake_minimum_required(VERSION 3.10)
project(a-travis-test)

add_executable(main main.cpp)

set(DSP_SRC
        thrid_party/kissfft/kiss_fft.c
        thrid_party/kissfft/kiss_fftr.c)

add_library(alib ${DSP_SRC})