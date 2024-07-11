cmake_minimum_required(VERSION 2.8)

project(RegExpAnalyzator)

set(SOURCE_EXE main.cpp)  #объявление переменной 

set(SOURCE_LIB RegExpAnalyze.cpp)	

add_library( RegExpAnalyze STATIC ${SOURCE_LIB})

add_executable(main ${SOURCE_EXE})

target_link_libraries(main RegExpAnalyze)	
