set(AKU_DIR ${SRC_DIR}/aku)

set(AKU_SRCS
	${AKU_DIR}/AKU.cpp
	${AKU_DIR}/AKU.h
)

set(AKU_PCH_SRCS
	pch.cpp
	pch.h
)

set(AKU_AUDIOSAMPLER_SRCS
	AKU-audiosampler.cpp
	AKU-audiosampler.h
)

set(AKU_DEBUGGER_SRCS
	AKU-debugger.cpp
	AKU-debugger.h
)

set(AKU_FMOD_SRCS
	AKU-fmod.cpp
	AKU-fmod.h
)

set(AKU_LUAEXT_SRCS
	AKU-luaext.cpp
	AKU-luaext.h
)

set(AKU_PARTICLES_SRCS
	AKU-particles.cpp
	AKU-particles.h
)

set(AKU_UNTZ_SRCS
	AKU-untz.cpp
	AKU-untz.h
)

add_library(aku ${AKU_SRCS})