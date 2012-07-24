set(MOAIZL_DIR ${SRC_DIR}/zlcore)

include_directories(${TLSF_DIR})

add_library(zlcore
	${MOAIZL_DIR}/ZLDirectoryItr.cpp
	${MOAIZL_DIR}/ZLFile.cpp
	${MOAIZL_DIR}/ZLFileSystem.cpp
	${MOAIZL_DIR}/ZLVirtualPath.cpp
	${MOAIZL_DIR}/ZLZipArchive.cpp
	${MOAIZL_DIR}/ZLZipStream.cpp
	${MOAIZL_DIR}/zl_mutex.cpp
	${MOAIZL_DIR}/zl_util.cpp
	${MOAIZL_DIR}/zl_vfscanf.cpp
	${MOAIZL_DIR}/zlcore-pch.cpp
	${MOAIZL_DIR}/zlcore.cpp
)