set(PROJECT_LIB_SRC
    prelude.cpp
)

add_library(${PROJECT_LIB_NAME} ${PROJECT_LIB_SRC})
target_include_directories(${PROJECT_LIB_NAME} PUBLIC ../include)
target_link_libraries(${PROJECT_LIB_NAME} glog::glog)
target_set_warnings(${PROJECT_LIB_NAME} ENABLE ALL)