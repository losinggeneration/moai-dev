set(MOAIZIPFS_DIR ${SRC_DIR}/zipfs)

include_directories(${TLSF_DIR})

add_library(zipfs
	${MOAIZIPFS_DIR}/ZIPFSString.c
	${MOAIZIPFS_DIR}/ZIPFSVirtualPath.c
	${MOAIZIPFS_DIR}/ZIPFSZipFile.c
	${MOAIZIPFS_DIR}/zipfs-pch.c
	${MOAIZIPFS_DIR}/zipfs.c
	${MOAIZIPFS_DIR}/zipfs_util.c
	${MOAIZIPFS_DIR}/zipfs_vfscanf.c
)