add_library(glslang-default-resource-limits
            ${CMAKE_CURRENT_SOURCE_DIR}/ResourceLimits.cpp)
set_property(TARGET glslang-default-resource-limits PROPERTY FOLDER glslang)
set_property(TARGET glslang-default-resource-limits PROPERTY POSITION_INDEPENDENT_CODE ON)

target_include_directories(glslang-default-resource-limits
                           PUBLIC ${CMAKE_CURRENT_SOURCE_DIR}
                           PUBLIC ${PROJECT_SOURCE_DIR})
