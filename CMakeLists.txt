cmake_minimum_required(VERSION 3.24)

set(CMAKE_TOOLCHAIN_FILE "${CMAKE_CURRENT_SOURCE_DIR}/vcpkg/scripts/buildsystems/vcpkg.cmake")

project(imgui1)

set(CMAKE_EXPORT_COMPILE_COMMANDS ON)

find_package(glfw3 CONFIG REQUIRED)
# target_link_libraries(main PRIVATE glfw)

find_package(Vulkan REQUIRED)
# target_link_libraries(main PRIVATE Vulkan::Vulkan)

find_package(imgui CONFIG REQUIRED)
# target_link_libraries(main PRIVATE imgui::imgui)

add_subdirectory(demo)

