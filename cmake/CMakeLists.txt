cmake_minimum_required(VERSION 2.6)

project(Moai)

set(TOPDIR ${CMAKE_SOURCE_DIR}/..)

set(THIRDPARTY_DIR ${TOPDIR}/3rdparty)
set(SRC_DIR ${TOPDIR}/src)

# third party
set(BOX2D_DIR ${THIRDPARTY_DIR}/box2d-2.2.1)
set(CHIPMUNK_DIR ${THIRDPARTY_DIR}/chipmunk-5.3.4)
set(CHIPMUNK_INC_DIR ${CHIPMUNK_DIR}/include)
set(JANSSON_DIR ${THIRDPARTY_DIR}/jansson-2.1/src)
set(JPEG_DIR ${THIRDPARTY_DIR}/jpeg-8c)
set(LUA_DIR ${THIRDPARTY_DIR}/lua-5.1.3/src)
set(OOID_DIR ${THIRDPARTY_DIR}/ooid-0.99)
set(TINYXML_DIR ${THIRDPARTY_DIR}/tinyxml)
set(TLSF_DIR ${THIRDPARTY_DIR}/tlsf-2.0)

# Find system packages that are not built in 3rdparty
find_package(Freetype REQUIRED)
find_package(OpenGL REQUIRED)

include_directories(${FREETYPE_INCLUDE_DIR_freetype2} ${OPENGL_INCLUDE_DIR})

add_subdirectory(3rdparty)
add_subdirectory(src)
