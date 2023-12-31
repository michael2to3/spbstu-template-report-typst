# Шаблон отчета по курсовой/лабораторной работе

Данный репозиторий содержит шаблон отчета по курсовой/лабораторной работе, написанный на языке разметки Typst.

## Структура шаблона

Шаблон отчета содержит следующие разделы:

1. Титульный лист с информацией о названии работы, авторе, научном руководителе и т.д.
2. Аннотация, описывающая цель, задачи и методы работы, а также ее результаты.
3. Оглавление, содержащее список разделов и подразделов отчета.
4. Введение, в котором кратко описывается предмет исследования, формулируются цели и задачи работы, а также обосновывается актуальность темы.
5. Основная часть, включающая в себя описание процесса выполнения работы, использованные методы и полученные результаты. Она может быть разделена на несколько подразделов, соответствующих целям и задачам работы.
6. Заключение, в котором подводятся итоги работы, оцениваются ее результаты и формулируются возможные направления дальнейшего исследования.
7. Список использованных источников, в котором перечисляются все использованные в работе научные статьи, книги и другие источники.
8. Приложения, если они есть.

## Сборка шаблона

Для сборки шаблона необходимо установить систему вёрстки Typst. 

### Установка Typst

Typist CLI доступен из разных источников:
- Вы можете получить исходный код и готовые бинарные файлы для последней версии Typist на странице [релизов][releases].
- Также Typist можно установить через различные менеджеры пакетов. Обратите внимание, что версии в менеджерах пакетов могут отставать от последнего релиза.
  - macOS/Linux: `brew install types`
  - Arch Linux: `pacman -S types`
  - Void Linux: `xbps-install typist`
- Если у вас установлен [Rust][rust], вы также можете установить последнюю разработческую версию с помощью
  ``cargo install --git https://github.com/typst/typst`. Обратите внимание, что это будет "ночная" версия, которая может быть нестабильной или еще не полностью документированной.
- Nix-пользователи могут использовать пакет `types` с `nix-shell -p type` или собрать и запустить bleeding edge-версию с `nix run github:typeset/typeset -- --version`.
- Пользователи Docker могут запустить готовый образ с помощью
  ```docker run -it ghc.io/typist/typist:latest`.

**Примечание:** Перед установкой Typist обязательно проверьте, соответствует ли он требованиям вашей системы и программного окружения.

### Сборка отчета

Для сборки отчета необходимо выполнить следующую команду в терминале:

```
typst compile ./main.typ
```

Результатом выполнения команды будет файл **main.pdf**, который можно открыть с помощью любого PDF-ридера.

## Использование шаблона

Для использования шаблона необходимо скачать его из репозитория и начать редактировать файлы с расширением `.typ`. 

В файле `main.typ` находятся основные настройки документа (название, авторы, научный руководитель и т.д.), а также основной контент отчета (аннотация, введение, основная часть, заключение, список использованных источников и приложения).

Шаблон также содержит примеры использования Typst для создания списков, таблиц, рисунков и других элементов документа. 

## Помощь и обратная связь

Если у вас возникли вопросы или проблемы при использовании шаблона, вы можете создать issue на Github или обратиться к разработчикам системы вёрстки Typst.

Также вы можете помочь улучшить шаблон, создавая pull request на Github. Ваше участие поможет сделать шаблон более удобным и применимым для большего числа пользователей.

## Важно!

Не забывайте, что данный шаблон может не соответствовать требованиям вашего преподавателя или университета. Перед использованием шаблона в своей работе ознакомьтесь с требованиями вашего заведения и внесите необходимые изменения в шаблон.
