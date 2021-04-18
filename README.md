# Работа с GIT и команды
### Настройка Git:
git config --global user.name "Vasya Pupkin"
git config --global user.email vasya@localhost
### Переход в простой редактор:
git config --global core.editor nano
## Репозиторий создаётся в конкретном каталоге с помощью команды:
$ git init
## Добавление файлов:
$ git add index.html
### Добавление всех файлов в текущем каталоге:
$ git add *
$ git add *.js →↓
### добавит в список отслеживаемых файлов все файлы срасширением .js в текущем каталоге и подкаталогах.
# Отслеживание статуса текущего директория:
$ git status
# Фиксация изменений:
$ git commit
# Добавление и коммит (Для новых add делаем отдельно):
$ git commit -a -m "Комментарий"
## История коммитов:
$ git log
## Полная версия коммитов:
$ git show <id-коммитта>
## Исправить ошибки, в случае если добавили ошибочно файл: 
$ git rm --cached stuff.txt
## Исправить коммит:
$ git commit --amend -m "Roboto Font"
## Добавить зеркальный коммит, который исправит предыдущий (без треуг.скобок):
$ git revert <commit-id> 
# КЛОНИРОВАНИЕ РЕПО С Github:
$ git clone https://...
# Команда git remote позволяет нам управлять удалёнными репозиториями (добавлять, удалять, просматривать).Например, мы можем в только что склонированном репозитории посмотреть remote: Общепринято, что первый удалённый репозиторий называют origin.
$ git remote -v origin https://github.com/netology-git/demo.git(fetch)originhttps://github.com/netology-git/demo.git(push)
# Подключаем удаленный репо к локальному (когда он у нас уже есть):
$ git remote add origin https://github.com/netology-git/demo.git
$ git remote -v 
    origin https://github.com/netology-git/demo.git (fetch)
    origin https://github.com/netology-git/demo.git (push)
## Отправка в удаленный репо push для первой отправки:
$ git push -u origin master
## Для последующих отправок:
$ git push
# MARKDAWN
* Обычный текст никакой специальной разметкой не оформляется.
Жирный, наклонный и перечёркнутый текст: **Жирный текст** *Наклонный текст* ~~Перечеркнутыйтекст~~
# Гиперссылки оформляются в формате:
[Текст ссылки] (http://localhost)
# Изображения оформляются так же, как и гиперссылки, но перед []ставится !, т.е. 
![логотип](url-изображения):# git
