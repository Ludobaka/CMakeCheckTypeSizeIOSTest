cmake_minimum_required (VERSION 3.14)
project (CheckTypeSizeIOSTest)

include (CheckTypeSize)
check_type_size ("int" SIZEOF_INT)
message("Sizeof int : ${SIZEOF_INT}")
