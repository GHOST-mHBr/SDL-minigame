cmake_minimum_required(VERSION 3.9)

project(Head-Football VERSION 0.1 DESCRIPTION "Simple game using SDL2" LANGUAGES CXX)

add_executable(Program main.cpp)

add_custom_command(
  TARGET Program POST_BUILD
  COMMAND cp -r ${CMAKE_CURRENT_SOURCE_DIR}/raw ${CMAKE_CURRENT_BINARY_DIR}
  VERBATIM
)


target_link_libraries(Program SDL2 SDL2_gfx SDL2_mixer SDL2_image SDL2_ttf)
