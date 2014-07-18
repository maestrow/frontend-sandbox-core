﻿# Frontend Sandbox 

Изучать всевозможные фреймворки и библиотеки удобно на примерах. 
Frontend Sandbox - это небольшая платформа для хостинга коллекции демонстрационных примеров frondtend-технологий. 


## Быстрый старт

- `node -v` должна быть [>= v0.11.9](http://nodejs.org/dist/)
- `npm install`
- `npm start`


## Демонстрационные модули

- Демонстрационные модули оформляются в виде отдельной папки и располагаются в `frontend/modules`. 
- На главной страничке (http://localhost:4000) автоматически формируется список всех модулей.
- Модуль состоит из файла макета `.html` (обязательно), кроме того можно добавить один или несколько `.js`-файлов. 
Имя файла макета должно совпадать с именем модуля (имя папки), имена `.js`-файлов могут быть произвольными.
- При переходе по адресу модудя (`http://localhost:4000/show/<ИмяМодуля>`) содержимое `.html`-файла будет вставлено в тэг `<body>` общего макета `views\master.ejs`. 
А `.js`-файлы, соответственно будут добавлены в теги `<script>`


## Пояснения

В качестве серверной web-платформы используется [Koa](https://github.com/koajs/koa) и, как следствие, требуется [>= Node v0.11.9](http://nodejs.org/dist/) и запуск Node с ключем `--harmony`, что уже указано в скрипте `start` в `package.json`.

> To use Koa you must be running node 0.11.9 or higher for generator support, and must run node(1) with the --harmony flag
