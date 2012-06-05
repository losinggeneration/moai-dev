set(HOSTS_DIR ${SRC_DIR}/hosts)

find_package(GLUT REQUIRED)
include_directories(${HOSTS_DIR} ${GLUT_INCLUDE_PATH})

set(FOLDERWATCHER_MAC_SRCS
	${HOSTS_DIR}/FolderWatcher-mac.h
	${HOSTS_DIR}/FolderWatcher-mac.mm
)

set(FOLDERWATCHER_WIN_SRCS
	${HOSTS_DIR}/FolderWatcher-win.cpp
	${HOSTS_DIR}/FolderWatcher-win.h
)

set(GLUTHOST_SRCS
	${HOSTS_DIR}/GlutHost.cpp
	${HOSTS_DIR}/GlutHost.h
)

set(GLUTHOST_MAIN
	${HOSTS_DIR}/GlutHostMain.cpp
)

set(PARTICLE_SRCS
	${HOSTS_DIR}/ParticlePresets.cpp
	${HOSTS_DIR}/ParticlePresets.h
)

add_library(gluthost ${GLUTHOST_SRCS})
target_link_libraries(gluthost ${GLUT_LIBRARIES})