ADD_SUBDIRECTORY(admst)


MACRO(adms_build_test arg1)
ADD_TEST(NAME ${arg1}_build
WORKING_DIRECTORY ${CMAKE_CURRENT_SOURCE_DIR}
COMMAND ${ADMST_SH} ${arg1}
)
ENDMACRO(adms_build_test)
### The test directories
ADD_SUBDIRECTORY(ekv)
ADD_SUBDIRECTORY(hicum0)
ADD_SUBDIRECTORY(hicum2)
ADD_SUBDIRECTORY(hicum2)
ADD_SUBDIRECTORY(mextram)
ADD_SUBDIRECTORY(psp102)