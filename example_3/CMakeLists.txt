cmake_minimum_required(VERSION 2.8) # Проверка версии CMake.
                                    # Если версия установленой программы
                                    # старее указаной, произайдёт аварийный выход.

project(hello_world)                # Название проекта

set(SOURCE_EXE main.cpp)            # Установка переменной со списком исходников

include_directories(foo)            # Расположение заголовочных файлов

add_executable(main ${SOURCE_EXE})  # Создает исполняемый файл с именем main
                                    # из исходника main.cpp

add_subdirectory(foo)               # Добавление подпроекта, указывается имя дирректории

target_link_libraries(main foo)     # Линковка программы с библиотекой
