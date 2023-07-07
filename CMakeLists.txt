cmake_minimum_required(VERSION 3.0.0)

project(ImGui LANGUAGES CXX)

add_library(ImGui STATIC
  "./imgui.cpp"
  "./imgui.h"
  "./imconfig.h"
  "./imgui_demo.cpp"
  "./imgui_draw.cpp"
  "./imgui_internal.h"
  "./imgui_tables.cpp"
  "./imgui_widgets.cpp"
  "./imstb_rectpack.h"
  "./imstb_textedit.h"
  "./imstb_truetype.h"
  "./backends/imgui_impl_sdl3.h"
  "./backends/imgui_impl_sdl3.cpp"
  "./backends/imgui_impl_sdlrenderer3.h"
  "./backends/imgui_impl_sdlrenderer3.cpp"
)

target_include_directories(ImGui PUBLIC ".")
