# Урок 1
## Работа с системой контроля версий
### 1. Иницилизация пустого репозитория
```
git init
```
### 2. Изменение пользовательской конфиигурации
```
git config --global user.name "Glebych"
git config --global user.email "glebych2@yandex.ru"
```
### 3. Создание файла исключений
```gitignore
# Файлы исключений
desktop.ini
Thumbs.db
.DS_Store
# Директория
.idea/
log/*
node_modules/
!/log/.htaccess
```
### 4. Добавление файлов в индексируемые
```
git add "file_name"
```
Индексируем все файлы в проекте за исключением тех, что орисаны в файле исключений
```
git add .
```
### 5. Убрать файлиз индексируемых
```
git rm -cashed "file_name"
```
### 6. Фиксация изменений
```
git commit -m "message"
```