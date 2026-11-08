# Лабораторная работа 1. Анализ карточной активности

## Содержание

- `01_analysis.ipynb` — очистка данных и исследование.
- `02_report.ipynb` — отчёт для руководителя.
- `report.pdf` — готовый отчёт.
- `cleaning_log.csv` — журнал решений по данным.
- `campaign_list.csv` — список клиентов для кампании.
- `clean_data.parquet` и `report_transactions_first.parquet` — очищенные данные для построения отчёта.

## Данные

Данные синтетические и выдаются отдельно. Для запуска первого ноутбука исходные файлы `clients.csv` и `transactions.csv` должны находиться в папке с ноутбуком.

## Запуск

Использовался Python 3.12. Для расчётов и экспорта нужны pandas, numpy, matplotlib, seaborn, pyarrow, Jupyter, nbconvert и Playwright.

1. Запустить `01_analysis.ipynb` сверху вниз.
2. Убедиться, что очищенные данные и файлы, необходимые отчёту, находятся рядом с `02_report.ipynb`.
3. Запустить `02_report.ipynb` сверху вниз.

Для сборки PDF в терминале:

`jupyter nbconvert --to webpdf --no-input --execute 02_report.ipynb --output report`

Для экспорта через webpdf также нужен установленный браузер Chromium для Playwright.
