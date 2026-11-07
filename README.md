# Итоговый проект: гибридная система рекомендаций книг (Goodbooks-10k)

**Решение — один файл: [`final_project.ipynb`](final_project.ipynb).** Он уже выполнен (таблицы, графики и выводы сохранены) и самодостаточен:
код модулей ноутбук записывает сам, поэтому кроме него нужен только датасет.

## Датасет

Goodbooks-10k (тот же, что в ДЗ №1): <https://www.kaggle.com/zygmunt/goodbooks-10k>.
Распакуйте CSV в папку `data/` рядом с ноутбуком:

```
final_project.ipynb
data/
├── books.csv
├── ratings.csv
├── tags.csv
├── book_tags.csv
└── to_read.csv        # необязателен
```

## Запуск

```bash
pip install numpy pandas scipy scikit-learn scikit-surprise torch lightgbm matplotlib seaborn jupyter nbconvert
jupyter lab final_project.ipynb        # Run All, ≈ 40–50 минут на CPU
```

Протестировано на Python 3.13; нужно ≈ 8 ГБ свободной оперативной памяти. Ноутбук сам создаст рядом папки `src/` (код), `outputs/` (метрики, графики, рекомендации) и `data_new_demo/`, `outputs_new_data/` (демонстрация запуска на новых данных) — вручную ничего делать не нужно.
