set(TRAIT_NAME "<YOUR TRAIT_NAME HERE>")

cmake_minimum_required(VERSION 3.10)
project(${TRAIT_NAME} LANGUAGES C)
add_library(${TRAIT_NAME} SHARED src/trait.c)
set_target_properties(${TRAIT_NAME} PROPERTIES
    C_VISIBILITY_PRESET default
    POSITION_INDEPENDENT_CODE ON
)
