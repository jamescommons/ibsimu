add_executable(simu)

find_package(PkgConfig REQUIRED)
pkg_check_modules(IBSIMU REQUIRED IMPORTED_TARGET GLOBAL ibsimu-1.0.6dev)

target_sources(simu
    PRIVATE
        vlasov2d.cpp
)

target_link_libraries(simu
    PUBLIC
        PkgConfig::IBSIMU
)
