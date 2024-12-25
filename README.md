# student-startpack
Простой сборщик на scss для студентов

**Version 1.1.2**

## Требования

Для работы необходимо наличие установленного ```node.js``` версии 18 и выше, и пакетного менеджера ```npm```.
Проверь это - введи по очереди команды:
```bash
node -v
```
```bash
npm -v
```
Если в ответ получил номера версий (для node - 18 или более ранняя) - все хорошо. Если нет - скачай и установи LTS версию [node.js](http://nodejs.org)
Вместе с **node.js** установиться пакетный менеджер **npm**

Установил нужную версию nodejs? Закрой и заново открой терминал. Повтори команды для проверки установленных версий node и npm - убедись, что версии подходят.

## Начало работы

**Форкни себе этот репозиторий и далее клонируй свой форк!**

1. Клонируй с указанием названия папки проекта (название проекта в конце через пробел):
```
git clone git@github.com:your-login-on-github/student-scss-pack.git project-name
```
Теперь на твоем компьютере есть локальный репозиторий созданный из этой заготовки

2. Перейди в папку только что склонированного репозитория:
```
cd project-name
```

3. Разорви связь между локальным репозиторием и удаленным, просто грохнув папку ```.git```:
```
rm -rf .git
```
теперь эта папка перестала быть гит репозиторием

4. Инициализируй в папке проекта git-репозиторий по новой:
```
git init
```

5. Создай пустой репозиторий на github под проект.

6. Привяжи локальный репозиторий к вновь созданному на гитхабе:
```
git remote add origin git@github.com:your-login-on-github/project-name.git
```
Это пример команды - точная команда/команды будут указаны в созданном пустом репозитории на гитхабе - ты создал его в предыдущем пункте.

7. Пушим в удаленный репозиторий на github:
```
git push -u origin master
```

8. Ставим зависимости:
```
npm install
```

## Запуск

В консоли выполняем команду:
```
npm run start
```
* Поднимается localhost
* В браузере автоматом открывается index.html
* Происходит отслеживание изменений в scss файлах и их пересборка
* Происходит отслеживание изменений в html файлах
* Происходит отслеживание изменений в js файлах
* При изменении перезагружается страница в браузере

## Структура папок и файлов
```
project
├───src
│   └───styles
│       ├───blocks (стили блоков)
│       │   ├───_header.scss
│       │   ├───_nav.scss
│       │   └───etc.
│       │
│       ├───common (общие стили)
│       │   ├───_fonts.scss
│       │   ├───_variables.scss
│       │   └───etc.
│       │
│       └───style.scss
│
└───www
    ├───fonts
    │   ├───font.woff2
    │   ├───font.woff
    │   └───etc.
    │
    ├───img
    │   ├───img.jpg
    │   └───etc.
    │
    ├───scripts
    │   ├───script.js
    │   └───etc.
    │
    ├───style
    │   └───style.css (собранный из scss файлов - его не трогаем)
    │
    ├───index.html
    ├───page1.html
    └───etc.
```

## Версии
* 1.1.2 - Скорректирован список зависимостей в package.json; обновлен readme.md
* 1.1.1 - Обновлены версии зависимостей для работы с nodejs 18 (LTS); обновлен readme.md
* 1.1.0 - Обновлены версии зависимостей для работы с nodejs 16 (LTS); обновлен readme.md
* 1.0.2 - изменен readme.md
* 1.0.1 - отслеживание изменений в js-файлах и перезагрузка страницы
* 1.0.0 - создание сборки