# CMakeLists.txt for building the Rust library

find_package(Cargo REQUIRED)

add_custom_target(rustlib ALL
    COMMAND cargo build --manifest-path ${CMAKE_CURRENT_SOURCE_DIR}/Cargo.toml
)
