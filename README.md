# Wildberries Data Cleaner
- Этот проект — мощный инструмент для обработки "битых" CSV-файлов Wildberries.
  Очищает данные, сортирует и сохраняет в трёх форматах с выравниванием и переносом текста.

## Пример результата
- ![Screenshot_20250406_184634](https://github.com/user-attachments/assets/23c9619b-f2e9-406d-af3a-ece4d2363d85)

## Возможности
- Очищает исходный файл, приводит числа к float: `Чистые_данные.csv/xlsx/pdf`.
- Выравнивает `Цена` и `Рейтинг` по центру, адаптирует ширину `Название` в Excel.
- Переносит длинные тексты `Название` и `Ссылка` в PDF.
- Сортирует по цене (от меньшего к большему): `Сортировка_по_цене.csv/xlsx/pdf`.
- Сортирует по рейтингу (от меньшего к большему, с учётом цены): `Сортировка_по_рейтингу.csv/xlsx/pdf`.
- Разделяет по рейтингам с сортировкой по цене: `Рейтинг_4.2.csv/xlsx/pdf` и т.д.
- Делит по ценовым диапазонам с сортировкой: `Цена_0_до_1000.csv/xlsx/pdf` и др.

## Требования
- Python 3.6+.
- Библиотеки: `pandas`, `openpyxl`, `reportlab`.
- Шрифт DejaVuSans (для PDF с кириллицей).

## Установка
- Проверьте Python: `python3 --version`
- Установите библиотеки: `pip3 install pandas openpyxl reportlab`
- Установите шрифт: `sudo apt install fonts-dejavu`
- Скачайте `wildberries_data_cleaner.py` и поместите рядом с `wildberries_data.csv`.

## Использование
- Перейдите в папку: `cd ~/Документы/3Пайтон`
- Запустите скрипт: `python3 wildberries_data_cleaner.py`
- Проверьте результаты в `wildberries_data_cleaner` (папки `CSV`, `Excel`, `PDF`).

## Структура проекта
- `wildberries_data_cleaner.py` — основной скрипт обработки.
- `README.md` — описание проекта.
- `.gitignore` — исключает временные файлы
- `LICENSE` — лицензия проекта.

## Автор
- Mangust-1981

## Лицензия
- MIT. Подробности в `LICENSE`.
