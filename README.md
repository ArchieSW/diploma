# Шаблон для курсовой в вышке с простым ci

## Курсовая

> Титульный лист: `title.tex`

> Основной файл: `coursework.tex`

Версия на английском и с использованием BibLatex в директории eng_biblatex. Если вы работаете в overleaf и файл `.bib` не подгружается может помочь создание копии проекта.

## Презентация к защите

> Файл: `slides.tex`

Презентацию тоже удобно делать в LaTeX. Для этого можно использовать класс `beamer`. Примеры презентаций этого класса:

1. https://www.overleaf.com/learn/latex/beamer
2. https://www.latextemplates.com/template/beamer-presentation

Для отрисовки схем и архитектур удобно использовать этот [tool](https://excalidraw.com).

## Сборка курсовой и презентации
1. Github Actions:
Сборка происходит автоматически при push в master. Готовые файлы будут доступны в артифактах к сборке
2. Локально:
Можно использовать [act](https://github.com/nektos/act) для сборки локально:
```
act push --artifact-server-path $PWD/.artifacts
```
Готовые файлы будут лежать в директории `.artifacts`
