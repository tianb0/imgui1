project(${CMAKE_PROJECT_NAME})

add_executable(demo main.cpp)

target_link_libraries(demo PRIVATE glfw)

target_link_libraries(demo PRIVATE Vulkan::Vulkan)

target_link_libraries(demo PRIVATE imgui::imgui)
