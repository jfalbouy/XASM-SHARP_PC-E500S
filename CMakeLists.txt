cmake_minimum_required(VERSION 3.20)
project(xasm-pc-e500s C)

set(CMAKE_C_STANDARD 17)
set(CMAKE_C_STANDARD_REQUIRED ON)
set(CMAKE_C_EXTENSIONS OFF)

include(GNUInstallDirs)

file(GLOB XASM_SOURCES src/xasm/*.C)
add_executable(xasm ${XASM_SOURCES})

target_include_directories(xasm PRIVATE ${CMAKE_CURRENT_SOURCE_DIR}/src/xasm)

install(TARGETS xasm RUNTIME DESTINATION ${CMAKE_INSTALL_BINDIR})
