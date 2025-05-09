set(srcs "main.c"
        "board.c")

idf_component_register(SRCS "${srcs}"
                    INCLUDE_DIRS  ".")
idf_build_set_property(PROJECT_KCONFIG_PROJBUILD ${CMAKE_CURRENT_SOURCE_DIR}/Kconfig.projbuild APPEND)