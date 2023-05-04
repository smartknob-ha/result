cmake_minimum_required(VERSION 3.16)
if(NOT ESP_PLATFORM)
  project(result VERSION 1.0.1 LANGUAGES CXX)
endif()

set(COMPONENT_ADD_INCLUDEDIRS "include")

if(ESP_PLATFORM)
  idf_component_register(INCLUDE_DIRS ${COMPONENT_ADD_INCLUDEDIRS})
endif()
