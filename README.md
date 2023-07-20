## Проект для изучения парсинга

> Парсер умеет собирать ссылки на статьи о нововведениях в Python, переходить по ним и забирать информацию об авторах и
> редакторах статей, собирать информацию о статусах версий Python, скачивать архив с актуальной документацией, а также 
> собирает данные обо всех PEP документах, сравнивает их статусы и сохраняет в csv-файл. 

## Технологии
Python и библиотеки BeautifulSoup4, Prettytable

### Как запустить проект:

Клонировать репозиторий и перейти в него в командной строке:

```
git clone git@github.com:shusharkin/bs4_parser_pep.git
```

```
cd bs4_parser_pep
```

Cоздать и активировать виртуальное окружение:

```
python3 -m venv мenv
```

```
source venv/Scripts/activate
```

Установить зависимости:

```
pip install -r requirements.txt
```

## Примеры команд

Справка
```
python main.py pep -h
```

Нововведения в Python:
```
python main.py whats-new
```

Последнии версии Python:
```
python main.py latest-versions -o pretty 
```

Спарсить данные обо всех документах PEP в csv-файл:
```
python main.py pep -o file
```