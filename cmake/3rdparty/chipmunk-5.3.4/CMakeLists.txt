include_directories(${CHIPMUNK_INC_DIR}/chipmunk)

add_library(chipmunk
	${CHIPMUNK_DIR}/src/chipmunk.c
	${CHIPMUNK_DIR}/src/constraints/cpConstraint.c
	${CHIPMUNK_DIR}/src/constraints/cpDampedRotarySpring.c
	${CHIPMUNK_DIR}/src/constraints/cpDampedSpring.c
	${CHIPMUNK_DIR}/src/constraints/cpGearJoint.c
	${CHIPMUNK_DIR}/src/constraints/cpGrooveJoint.c
	${CHIPMUNK_DIR}/src/constraints/cpPinJoint.c
	${CHIPMUNK_DIR}/src/constraints/cpPivotJoint.c
	${CHIPMUNK_DIR}/src/constraints/cpRatchetJoint.c
	${CHIPMUNK_DIR}/src/constraints/cpRotaryLimitJoint.c
	${CHIPMUNK_DIR}/src/constraints/cpSimpleMotor.c
	${CHIPMUNK_DIR}/src/constraints/cpSlideJoint.c
	${CHIPMUNK_DIR}/src/cpArbiter.c
	${CHIPMUNK_DIR}/src/cpArray.c
	${CHIPMUNK_DIR}/src/cpBB.c
	${CHIPMUNK_DIR}/src/cpBody.c
	${CHIPMUNK_DIR}/src/cpCollision.c
	${CHIPMUNK_DIR}/src/cpHashSet.c
	${CHIPMUNK_DIR}/src/cpPolyShape.c
	${CHIPMUNK_DIR}/src/cpShape.c
	${CHIPMUNK_DIR}/src/cpSpace.c
	${CHIPMUNK_DIR}/src/cpSpaceComponent.c
	${CHIPMUNK_DIR}/src/cpSpaceHash.c
	${CHIPMUNK_DIR}/src/cpSpaceQuery.c
	${CHIPMUNK_DIR}/src/cpSpaceStep.c
	${CHIPMUNK_DIR}/src/cpVect.c
)

set_target_properties(chipmunk
	PROPERTIES COMPILE_FLAGS -std=gnu99
)