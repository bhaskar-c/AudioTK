
FILE(GLOB
  ATK_DYNAMIC_TEST_SRC
  *.cpp
)

FILE(GLOB
  ATK_DYNAMIC_TEST_HEADERS
  *.h*
)

SET(ATK_DYNAMIC_TEST_DEFINITIONS)
SET(ATK_DYNAMIC_TEST_INCLUDE)
SET(ATK_DYNAMIC_TEST_LIBRARIES ATKDynamic ATKTools ATKMock ATKCore ${Boost_UNIT_TEST_FRAMEWORK_LIBRARY})

SET(ATK_DYNAMIC_TEST_NAME ATKDynamic_test)
SET(ATK_DYNAMIC_TEST_TESTNAME Dynamic)
SET(ATK_DYNAMIC_TEST_FOLDER Dynamic_test)

ATK_add_test(ATK_DYNAMIC_TEST)
