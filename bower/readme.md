
## Bower - менеджер пакетов ##

Официальный сайт: https://bower.io    
Хороший мануал: http://nano.sapegin.ru/all/bower  

#### Основные команды Bower ####

```sh 
npm install bower -g    // Установка ( -g означает глобально)
bower init              // Интерактивное создание конфиг-файла "bower.json"
bower -v                // Версия
bower search jquery     // Поиск
bower s jquery          // Поиск (сокращенно) 
bower info jquery       // Детальная информация о библиотеке 
```

#### Установка пакетов: ####

Установка пакетов по умолчанию производится в папку **"bower_components"** текущего каталога

```sh 
bower install <package>  // Установка пакета
bower i <package>        // Установка пакета (сокращенный синтаксис) 

// Ключи (чтобы отметить зависимости в "bower.json" )
-S, --save
-D, --save-dev
```

#### Примеры установки библиотек #### 
```sh 
bower install jquery#1.6.4 --save    // Установка определенной версии
bower i normalize.css                // Установка файла для CSS сброса 
bower install https://code.jquery.com/jquery-3.2.1.min.js  // Загрузка файла по ссылке

bower list                           // Просмотр списка установленных библиотек
bower list --path                    // Получение ссылок на уже скаченные библиотеки

bower uninstall jquery-3.2.1 --save  // Удаление библиотеки (отмечаем запись в bower.json)
bower list                           // Проверим что удалили (выведем список)
```

