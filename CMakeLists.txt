cmake_minimum_required( VERSION 3.12 FATAL_ERROR )

project( pkg2zip )

add_executable( "pkg2zip" 
    "${CMAKE_CURRENT_SOURCE_DIR}/pkg2zip.c"

    "${CMAKE_CURRENT_SOURCE_DIR}/miniz_tdef.c"
    "${CMAKE_CURRENT_SOURCE_DIR}/miniz_tdef.h"

    "${CMAKE_CURRENT_SOURCE_DIR}/pkg2zip_aes_x86.c"
    "${CMAKE_CURRENT_SOURCE_DIR}/pkg2zip_aes.c"
    "${CMAKE_CURRENT_SOURCE_DIR}/pkg2zip_aes.h"

    "${CMAKE_CURRENT_SOURCE_DIR}/pkg2zip_crc32_x86.c"
    "${CMAKE_CURRENT_SOURCE_DIR}/pkg2zip_crc32.c"
    "${CMAKE_CURRENT_SOURCE_DIR}/pkg2zip_crc32.h"

    "${CMAKE_CURRENT_SOURCE_DIR}/pkg2zip_out.c"
    "${CMAKE_CURRENT_SOURCE_DIR}/pkg2zip_out.h"

    "${CMAKE_CURRENT_SOURCE_DIR}/pkg2zip_psp.c"
    "${CMAKE_CURRENT_SOURCE_DIR}/pkg2zip_psp.h"

    "${CMAKE_CURRENT_SOURCE_DIR}/pkg2zip_sys.c"
    "${CMAKE_CURRENT_SOURCE_DIR}/pkg2zip_sys.h"

    "${CMAKE_CURRENT_SOURCE_DIR}/pkg2zip_utils.h"

    "${CMAKE_CURRENT_SOURCE_DIR}/pkg2zip_zip.c"
    "${CMAKE_CURRENT_SOURCE_DIR}/pkg2zip_zip.h"

    "${CMAKE_CURRENT_SOURCE_DIR}/pkg2zip_zrif.c"
    "${CMAKE_CURRENT_SOURCE_DIR}/pkg2zip_zrif.h"

    "${CMAKE_CURRENT_SOURCE_DIR}/puff.h"
    "${CMAKE_CURRENT_SOURCE_DIR}/puff.c"
)

set_property( DIRECTORY PROPERTY VS_STARTUP_PROJECT "pkg2zip" )