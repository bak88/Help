* Создание репозитория 
```sh
git init
```
* Настройки конфигурации
```sh
git config --global user.name "name"
git config --global user.email "email"
```
* Значение параметров конфигурации
```sh
git config --list
```
* Все параметры команды config
```sh
git config -h
```
* Добавление в индекс
```sh
git add <name_file>
git add .
```
* Сохранение изменений в репозиторий
```sh
git commit -m "Message"
```
* Просмотр сохранений
```sh
git show <номер индефикатора>
git show --pretty=fuller
```
* Выборочное добавление в индекс
```sh
git add -p <name_file>
```
* Сохранение всех изминений, но лишь в проиндексированых файлах
```sh
git commit -am "Message"
git commit -m "Message" name_file
```
* Удаление из директория
```sh
git rm -r name_file
```
* Удаление из индекса
```sh
git rm -r --cached name_file
```
* Удаление из рабочей директории и индекса
```sh
git rm -f name_file
```
* Переименование файлов
```sh
git mv name_file new_name_file
```
* Просмотр веток
```sh
git branch
git branch -v
```
* Создание новой ветки 
```sh
git branch name_branch
git checkout -b name_branch
```
* Переклюение по веткам
```sh
git checkout name_branch
```
* Удалить не закоммиченные изминения
```sh
git checkout -f name_branch or HEAD
```
* Сохранить не оконченные изминения и перход к ним
 ```sh
git stash
git stash pop - возврат к изминениям
```
* Перенос веток
```sh
git branch -f name_branch <индификатор коммита> или <имя ветки> - HEAD должна уйти с ветки
git checkout -B name_branch <индификатор коммита>
```

Пример:

git branch -f master 4282 - ветка master уйдет на коммит

git branch -f master new  - ветка master уйдет на ветку new 

git checkout -B master 4282 - команда передвинет ветку, а после переключится и все изменения останутся в прошлой ветке

* Слияние веток и отмена слияния
```sh
git merge
git branch -f master ORIG_HEAD
```
* Удаление веток
```sh
git branch -d <name_branch>
```
