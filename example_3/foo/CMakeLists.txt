cmake_minimum_required(VERSION 2.8)     # Проверка версии CMake.
                                        # Если версия установленой программы
                                        # старее указаной, произайдёт аварийный выход.

project(foo)                            # Название проекта

set(SOURCE_LIB foo.cpp)                 # Установка переменной со списком исходников

add_library(foo STATIC ${SOURCE_LIB})   # Создание статической библиотеки
