# TapeSorter
TapeSorter — это программа для для сортировки наборов данных, которые не помещаются в оперативной памяти. Она использует ленты (файлы) для хранения данных и выполняет сортировку с использованием промежуточных файлов.

## Структура проекта
- tape.h, tape.cpp — классы FileTape и TapeSorter, реализующие интерфейс ленты и алгоритм сортировки соответственно.
- test.cpp — тесты для проверки корректности работы программы.
- parser.h, parser.cpp — парсер аргументов командной строки.

## Аргументы командной строки
Программа принимает следующие аргументы командной строки:
- -i или --input — путь к входной ленте.
- -o или --output — путь к выходной ленте.
- После этого необходимо указать путь(и) к временным лентам (файлам), которые будут использоваться в процессе сортировки. Т.к. в реальной ситуации мы используем уже существующие ленты, было принято решение передавать их в качестве аргументов.

## Конфигурация
Конфигурационный файл - config.txt
- read_delay - задержка чтения из файла.
- write_delay - задержка записи в файл. 
- forward_delay - задержка иттерации вперёд.
- backward_delay - задержка иттерации назад.
