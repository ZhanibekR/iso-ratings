# Рейтинги IMO

## О проекте

РНПЦ Дарын [декларирует](https://daryn.kz/о-центре/), что «в рейтинге международного олимпийского движения на международных предметных олимпиадах (IMO, IPHO, ICHO, IBO, IOI) в 2017 году Казахстан занял 10-ю позицию среди 123 стран-участниц».

Этим проектом мы предлагаем проверить фактическую точность такого утверждения.

## Как добавить новый предмет?

В первую очередь надо написать парсер, обозвать его названием предмета и положить в папку `parsers`. В этом файле должна быть функция `export_ratings_based_on_score` которая принимает в качестве аргумента итерируемый объект (tuple/list), в котором каждый элемент это двухбуквенное обозначение страны (расшифровка есть в файле `helpers/country_codes.py`) и возвращает словарь (dict) в котором каждый ключ (это год в формате str) соотносится с другим словарем, где двухбуквенные обозначения стран соотносятся с местом страны в том году. Отдельно есть ключ `'total', который указывает общее кол-во стран-участниц.
