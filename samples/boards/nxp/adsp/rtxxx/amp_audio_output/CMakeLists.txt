# Copyright 2025 NXP
# SPDX-License-Identifier: Apache-2.0

cmake_minimum_required(VERSION 3.20.0)

find_package(Zephyr HINTS $ENV{ZEPHYR_BASE})

project(amp_audio_output)
target_sources(app PRIVATE src/main.c)

include("${CMAKE_CURRENT_LIST_DIR}/../common/dsp-load.cmake")
