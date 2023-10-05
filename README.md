## Asynchronous PEP documentation parser in Python - Асинхронный парсер документации PEP на Python.

### Описание:
Проект созданный для парсинга документации языка программирования Python. Проект реализован с помощью библиотеки "Scrapy" что позволяет добиться асинхронной работы. Вывод результатов производится в csv файл.

### Технологии :
![Python](https://img.shields.io/badge/Python-3.7-blue) ![Scrapy](https://img.shields.io/badge/Scrapy-2.5.1-blue) 
### Функционал:
Парсер анализирует статус всех PEP документов языка Python, и выводит информацию об них в два файла формата csv:
1.  В первом файле выводится список всех PEP: номер, звание и статус.
2.  Во втором файле выводится сводка по статусам PEP — сколько найдено документов в каждом статусе (статус, количество), а так же выводится общее количество найденных PEP документов.

### Как запустить проект:
Склонировать репозиторий в командной строке:
```bash
git clone https://github.com/IvanFilippov74/scrapy_parser_pep.git
```
Затем перейдите в корневую директорию проекта:
```bash
cd  scrapy_parser_pep/
```
Cоздать и активировать виртуальное окружение:
```bash
python3 -m venv venv
source venv/bin/activate
python3 -m pip install --upgrade pip
```
Установить зависимости из файла requirements.txt:
```bash
pip install -r requirements.txt
```
Запустите парсер командой:
```bash
scrapy crawl pep
```
Результаты парсинга можно увидеть в директории /results/ :
```
├── results/
   ├── pep_2023-10-05T07-51-34.csv
   └── status_summary_2023-10-05T12-52-00.csv
```

### Авторы:
Filippov Ivan<br>
<a href="https://github.com/IvanFilippov74"><img src="https://img.shields.io/badge/github-%23121011.svg?style=for-the-badge&logo=github&logoColor=white"></a>