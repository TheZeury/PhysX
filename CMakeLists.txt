set (PHYSX_ROOT_DIR "physx/")
set (CMAKEMODULES_PATH "dependencies/CMakeModules/")
set (CMAKEMODULES_NAME "CMakeModules")
set (CMAKEMODULES_VERSION "1.27")
set (TARGET_BUILD_PLATFORM windows)
set (PHYSX_SLN_PHYSXDEVICE_PATH "dependencies/PhysXDevice/")
set (PHYSX_SLN_FREEGLUT_PATH "dependencies/freeglut-windows/")
set (PX_OUTPUT_LIB_DIR "${CMAKE_CURRENT_BINARY_DIR}/external/physx/")
set (PX_OUTPUT_BIN_DIR "${CMAKE_CURRENT_BINARY_DIR}/external/physx/")

add_subdirectory (physx/compiler/public)

set (PHYSX_LIBRARIES 
	PhysX
	PhysXCharacterKinematic
	PhysXCommon
	PhysXCooking
	PhysXExtensions
	PhysXFoundation
	PhysXVehicle
)