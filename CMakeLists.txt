cmake_minimum_required(VERSION 3.30)
project(Contenedores)

set(CMAKE_CXX_STANDARD 20)

find_package(Boost REQUIRED)

# Incluye los directorios de Boost.
include_directories(${Boost_INCLUDE_DIRS})

add_executable(CPP_Contenedores_Dinamicos
        main.cpp

)
target_link_libraries(CPP_Contenedores_Dinamicos ${Boost_LIBRARIES})
