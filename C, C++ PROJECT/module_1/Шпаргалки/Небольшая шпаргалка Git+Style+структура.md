# Основные команды

## Создание структуры проекта
```sh
mkdir -p src
```

## Компиляция и запуск программы
```sh
gcc -Wall -Werror -Wextra -std=c11 -o hello src/hello.c
```

## Следование стилевой норме Google C++ Style Guide
```
BasedOnStyle: Google
Language: Cpp
Standard: Cpp11
```

## Создайте файл hello.c в директории src:
```sh
touch src/hello.c
```

## Запуск программы:
```
./hello
```

## Проверка стиля кода
```sh
clang-format -i src/hello.c
```

# Работа с git
## Инициализируйте репозиторий git, если он еще не инициализирован:
```sh
git init
```

##  Создайте ветку develop:
```sh
git checkout -b develop
```

## Добавьте и закоммитьте файл hello.c
```sh
git add src/hello.c
git commit -m "Add hello.c with 'Hello, AI!' output"
```

## Опубликуйте изменения в удалённый репозиторий
```sh
git remote add origin <URL вашего репозитория>
git push -u origin develop
```