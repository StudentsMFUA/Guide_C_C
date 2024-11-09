# Основные команды

## Создание структуры проекта
```bash
mkdir -p src
```

## Компиляция и запуск программы
```bash
gcc -Wall -Werror -Wextra -std=c11 -o hello src/hello.c
```

## Следование стилевой норме Google C++ Style Guide
```
BasedOnStyle: Google
Language: Cpp
Standard: Cpp11
```

## Создание файла hello.c в директории src:
```bash
touch src/hello.c
```

## Запуск программы:
```
./hello
```

## Проверка стиля кода
```bash
clang-format -i src/hello.c
```

# Работа с git
## Инициализируйте репозиторий git, если он еще не инициализирован:
```bash
git init
```

##  Создайте ветку develop:
```bash
git checkout -b develop
```

## Добавьте и закоммитьте файл hello.c
```bash
git add src/hello.c
git commit -m "Add hello.c with 'Hello, AI!' output"
```

## Опубликуйте изменения в удалённый репозиторий
```bash
git remote add origin <URL вашего репозитория>
git pubash -u origin develop
```