if (NOT MSVC)
	set(CMAKE_C_FLAGS "${CMAKE_C_FLAGS} -std=gnu99")
endif()

set(FILES
	internal.c
	wshash.h
	endian.h
	compiler.h
	fnv.h
	data_sizes.h
	sha3.c
	sha3.h
)

add_library(wshash ${FILES})

