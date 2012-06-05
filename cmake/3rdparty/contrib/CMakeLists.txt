set(CONTRIB_DIR ${THIRDPARTY_DIR}/contrib)

set(CONTRIB_SRCS
	${CONTRIB_DIR}/utf8.c
	${CONTRIB_DIR}/utf8.h
)

add_library(contrib ${CONTRIB_SRCS})