set(MOAI_DIR ${SRC_DIR}/moai)

set(MOAI_SRCS
	${MOAI_DIR}/main.cpp
)

add_executable(moai ${MOAI_SRCS})

target_link_libraries(moai
	aku
	gluthost
	moaicore
	uslscore
	zipfs

# 3rd party
	chipmunk
	box2d
	contrib

# System (to have cmake added)
	GLEW
	crypto
	curl
	freetype
	jansson
	jpeg
	lua
	png
	ssl
	tinyxml
	tlsf
	z

# System without 3rd-party library
	GL
	pthread
	rt
)