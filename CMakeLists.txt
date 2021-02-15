cmake_minimum_required(VERSION 3.17.0)

if (NOT LT_PROJECT_INIT)
    include(submodule/pesto/cmake/lt_cmake_common.cmake)
endif ()

lt_project_init(TOOLCHAIN gcc-9.2.0)
project(rapidjson)
lt_init_packages()

lt_create_interface(rapidjson
        NAMESPACE rapidjson
        )

lt_setup()