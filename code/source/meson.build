code = files('example.c')

lib = static_library('fscl-stm32xx-x-c',
    code,
    include_directories: dir)

fscl_stm32xx_x_dep = declare_dependency(
    link_with: lib,
    include_directories: dir)
