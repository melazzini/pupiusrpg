aux_source_directory(
    "${CMAKE_CURRENT_SOURCE_DIR}/src"
    _TUNITS_ROOT_SRC) # source files in the ./src subdirectory

add_executable(app "")

target_sources(app PRIVATE "${_TUNITS_ROOT_SRC}")

target_include_directories(app PRIVATE inc)

target_link_libraries(app fmt)