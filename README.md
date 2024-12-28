
# VShell

**VShell** — это виртуальная оболочка, которая работает с виртуальной файловой системой, представленной в виде zip-архива. Она поддерживает команды для навигации по каталогам, вывода содержимого файлов, а также выполнение простых скриптов.

## Структура проекта

```
vshell/
├── vshell.py          # Основной файл программы с реализацией виртуальной оболочки
├── test_vfs.zip       # Пример виртуальной файловой системы (zip-архив)
├── test_config.xml    # Конфигурационный файл для программы
├── tests.py           # Тесты для программы
README.md             # Этот файл
```

## Как склонировать репозиторий

1. Склонируйте репозиторий с помощью Git:

```bash
git clone <URL репозитория>
cd <папка с проектом>
```

2. Убедитесь, что у вас установлен Python 3.x.

## Как запустить программу

1. Убедитесь, что у вас есть конфигурационный файл и виртуальная файловая система:

- Конфигурационный файл (`test_config.xml`)
- Виртуальная файловая система (`test_vfs.zip`)

2. Запустите программу, указав конфигурационный файл как аргумент:

```bash
python vshell.py test_config.xml
```

Программа предложит командную строку, где можно вводить команды, такие как `ls`, `cd`, `head`, `tac`, и `exit`.

## Как запустить тесты

1. Для запуска тестов используйте `unittest`:

```bash
python -m unittest tests.py
```

Тесты проверят основные команды оболочки, такие как навигация по каталогам, вывод содержимого файлов и корректность работы команды `exit`.
