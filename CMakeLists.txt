cmake_minimum_required(VERSION 3.2)

#cpm
set(CPM_MODULE_NAME "ofxiOSBoost")
set(CPM_LIBRARIES ${CPM_LIBRARIES} ${CMAKE_CURRENT_SOURCE_DIR}/libs/boost/ios/libboost.a)
CPM_ExportAdditionalIncludeDir(libs/boost/include/)
include(cpm_bootstrap.cmake)

CPM_InitModule(${CPM_MODULE_NAME})

#add_custom_target(libs/boost/ios/libboost.a)