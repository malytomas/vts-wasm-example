
cmake_minimum_required(VERSION 3.10)

add_subdirectory(browser)

# override memory limits
set_property(TARGET vts-browser-wasm-canvas APPEND PROPERTY LINK_FLAGS "-s TOTAL_MEMORY=512MB -s WASM_MEM_MAX=1GB")


