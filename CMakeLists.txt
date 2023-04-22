set (PHYSX_ROOT_DIR "${CMAKE_CURRENT_SOURCE_DIR}/physx")
set (CMAKEMODULES_PATH "${CMAKE_CURRENT_SOURCE_DIR}/dependencies/CMakeModules/")
set (CMAKEMODULES_NAME "CMakeModules")
set (CMAKEMODULES_VERSION "1.27")
set (TARGET_BUILD_PLATFORM windows)
set (PHYSX_SLN_PHYSXDEVICE_PATH "${CMAKE_CURRENT_SOURCE_DIR}/dependencies/PhysXDevice/bin/x86")
set (PHYSX_SLN_FREEGLUT_PATH "${CMAKE_CURRENT_SOURCE_DIR}/dependencies/freeglut-windows/bin")
set (PHYSX_SLN_PHYSXGPU_PATH "${CMAKE_CURRENT_SOURCE_DIR}/dependencies/PhysXGpu") # not exiting yet.
set (GPU_DLL_COPIED 1) # not using it yet.
set (PX_OUTPUT_LIB_DIR "${CMAKE_CURRENT_BINARY_DIR}")
set (PX_OUTPUT_BIN_DIR "${CMAKE_CURRENT_BINARY_DIR}")

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