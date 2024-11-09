CMAKElists.txt
cmake_minimum_required(VERSION 3.10)

# Название вашего проекта
project(untitled C)

# Установка стандартного флага компиляции
set(CMAKE_C_STANDARD 11)

# Добавление флагов компилятора
add_compile_options(-Wall -Wextra -Werror)

# Добавление исполняемого файла
add_executable(untitled main.c)

shift+command+h // в Finder переход в home директорию