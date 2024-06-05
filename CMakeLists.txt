cmake_minimum_required(VERSION 3.5)

project(GhostwriterMath LANGUAGES CXX)

set(CMAKE_CXX_STANDARD 17)
set(CMAKE_CXX_STANDARD_REQUIRED ON)

add_executable(GhostwriterMath main.cpp)

include(GNUInstallDirs)
install(TARGETS GhostwriterMath
    LIBRARY DESTINATION ${CMAKE_INSTALL_LIBDIR}
    RUNTIME DESTINATION ${CMAKE_INSTALL_BINDIR}
)
