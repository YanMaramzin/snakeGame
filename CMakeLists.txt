cmake_minimum_required(VERSION 3.30)
project(snakeGame)

set(CMAKE_CXX_STANDARD 20)

set(CMAKE_CXX_STANDARD_REQUIRED ON)
set(CMAKE_CXX_EXTENSIONS OFF)
set(CMAKE_EXPORT_COMPILE_COMMANDS ON)
add_subdirectory(thirdParty)

add_executable(snakeGame main.cpp)

target_link_libraries(${PROJECT_NAME}
        PRIVATE ftxui::screen
        PRIVATE ftxui::dom
        PRIVATE ftxui::component  # Not needed for this example.
)
