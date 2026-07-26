# Анализ структурных особенностей ДНК (GC-Content)
## Описание проекта
Данный проект представляет собой разведочный анализ данных (EDA) синтетического датасета биологических образцов ДНК. Основная цель исследования — выявить закономерности в распределении содержания гуанина и цитозина (GC-Content) в зависимости от типа организма (`Class_Label`) и уровня риска заболевания (`Disease_Risk`), а также оценить пригодность этого признака для первичной классификации.

В ходе работы были проведены очистка данных, статистический анализ, визуализация и создание интерактивного дашборда в Yandex DataLens.

## Ссылки на материалы
*   **Исходные данные:** [Kaggle: DNA Classification Dataset](https://www.kaggle.com/datasets/miadul/dna-classification-dataset)
*   **Код анализа (Notebook):** [GitHub: dna_analysis_notebook.ipynb](https://github.com/akava-pink/my-first-project/blob/main/dna_analysis_notebook.ipynb)
*   **Очищенный датасет:** [Google Drive: synthetic_dna_dataset_cleaned.csv](https://drive.google.com/drive/u/0/folders/19THvs_dho_rB8WyfXhDoeh16D1FlDCm3)
*   **Интерактивный дашборд:** [Yandex DataLens Dashboard](https://datalens.yandex/lcb6p7n77p404)

## Структура файлов проекта
Проект организован по стандарту, обеспечивающему прозрачность и воспроизводимость результатов:

```text
project_name/
── data_raw/                  # Исходные необработанные данные
│   └── synthetic_dna_dataset.csv
├── data_clean/                # Очищенные и подготовленные данные
│   └── synthetic_dna_dataset_cleaned.csv
── notebooks/                 # Jupyter Notebook с кодом анализа
│   └── dna_analysis_notebook.ipynb
├── outputs/                   # Итоговые таблицы агрегаций
│   ├── stats_by_class_label.csv
│   ── correlation_matrix_numeric.csv
├── charts/                    # Сохраненные графики (PNG)
│   ├── hist_gc_content_distribution.png
│   ├── boxplot_class_gc.png
│   └── bar_chart_mean_gc.png
├── reports/                   # Текстовые отчеты
│   └── Analytical_Report_DNA_GC_Content.md
└── README.md                  # Инструкция по запуску проекта
