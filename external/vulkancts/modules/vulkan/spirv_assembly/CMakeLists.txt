# SPIR-V assembly tests

include_directories(..)

set(DEQP_VK_SPIRV_ASSEMBLY_SRCS
	vktSpvAsmComputeShaderCase.cpp
	vktSpvAsmComputeShaderCase.hpp
	vktSpvAsmComputeShaderTestUtil.cpp
	vktSpvAsmComputeShaderTestUtil.hpp
	vktSpvAsmGraphicsShaderTestUtil.cpp
	vktSpvAsmGraphicsShaderTestUtil.hpp
	vktSpvAsmInstructionTests.cpp
	vktSpvAsmInstructionTests.hpp
	vktSpvAsmTests.cpp
	vktSpvAsmTests.hpp
	)

set(DEQP_VK_SPIRV_ASSEMBLY_LIBS
	tcutil
	vkutil
	)

add_library(deqp-vk-spirv-assembly STATIC ${DEQP_VK_SPIRV_ASSEMBLY_SRCS})
target_link_libraries(deqp-vk-spirv-assembly ${DEQP_VK_SPIRV_ASSEMBLY_LIBS})
