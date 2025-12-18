# Snakemake

## 1. Клонирование репозитория

```bash
git clone https://github.com/https://github.com/AnnaToropova/Snakemake.git
```

### Перейти в каталог проекта:

```bash
cd snakemake
```

## 2. Проверка Python

```bash
py --version
```

Ожидаемый вывод, например:

```bash
Python 3.11.9
```

## 3. Установка Snakemake

```bash
py -m pip install --upgrade pip
py -m pip install snakemake
```

## 4. Проверка установки Snakemake

```bash
py -m snakemake --version
```

Ожидаемый вывод, например:

```bash
9.14.5
```

## 5. Dry-run (проверка workflow без выполнения)

```bash
py -m snakemake -n
```

Ожидаемый вывод:

```bash
rule process_text:
    input: data/input.txt
    output: results/output.txt
```

## 6. Запуск workflow

```bash
py -m snakemake --cores 1
```

## 7. Проверка результата

```bash
type results\output.txt
```

Ожидаемый вывод:

```bash
=== Статистика текста ===
Строк: 4
Слов: 69
Символов: 448

=== Обработанный текст в верхний регист ===
LOREM IPSUM DOLOR SIT AMET, CONSECTETUR ADIPISCING ELIT, SED DO EIUSMOD TEMPOR INCIDIDUNT UT LABORE ET DOLORE MAGNA ALIQUA. 
UT ENIM AD MINIM VENIAM, QUIS NOSTRUD EXERCITATION ULLAMCO LABORIS NISI UT ALIQUIP EX EA COMMODO CONSEQUAT. 
DUIS AUTE IRURE DOLOR IN REPREHENDERIT IN VOLUPTATE VELIT ESSE CILLUM DOLORE EU FUGIAT NULLA PARIATUR. 
EXCEPTEUR SINT OCCAECAT CUPIDATAT NON PROIDENT, SUNT IN CULPA QUI OFFICIA DESERUNT MOLLIT ANIM ID EST LABORUM.
```
