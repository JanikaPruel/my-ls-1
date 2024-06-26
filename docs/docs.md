### Понимание задания

Проект `my-ls` требует реализации собственной версии команды `ls` на языке Go. Команда `ls` отображает файлы и папки в указанной директории. Если директория не указана, отображается содержимое текущей директории. Ваша реализация должна поддерживать следующие флаги:
- `-l`: длинный формат вывода
- `-R`: рекурсивный просмотр каталогов
- `-a`: отображение всех файлов, включая скрытые
- `-r`: обратный порядок сортировки
- `-t`: сортировка по времени модификации


### Подробное описание файлов и папок

#### `cmd/`
- Содержит директории с основными программами.

##### `cmd/my_ls/main.go`
- Основной файл для программы `my-ls`.

#### `internal/`
- Содержит внутренние пакеты, не предназначенные для использования вне этого проекта.

##### `internal/flags/`
- Содержит логику для работы с флагами командной строки.

###### `flags.go`
- Реализация парсинга флагов и проверки их комбинаций.


##### `internal/ls/`
- Содержит логику для выполнения основной функциональности `ls`.

###### `ls.go`
- Реализация команд `ls`, включая поддержку флагов.


##### `internal/utils/`
- Содержит вспомогательные функции и утилиты.

###### `utils.go`
- Вспомогательные функции для работы с файлами и строками.

