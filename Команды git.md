### Команды Git
----

#### В консоли

dir - показывает все папки
tree - дерево папок
cd desktop - переход в папку рабочий стол
cd.. - возвращает назад в папку
MD - создание нового каталога
RD - удаление каталога
type nul > hello.txt - создание файла 
"hello.txt" - открывает файл
ren blag.txt blog.txt - переименовывание файла
DEL - удаление одного или нескольких файлов
code . - запускает vscode
`copy file1.txt e:\tmp\newfile.txt` - копирование файла и смена имени
CLS - очистка экрана в командной строке

---

#### Работа с git

git init - инциализация гита
git status -  отображает состояние рабочего каталога и раздела проиндексированных файлов.
git add index.html - добавляет содержимое рабочей директории в индекс (staging area) для последующего коммита.
git rm --cached index.html - удаляет содержимое
git add . - добавляет все файлы из рабочего каталога
git commit -m "first commit" - задает сообщение коммита, нужно чтобы описать изменения

git branch -M main - переименовывает master в main
git branch - список веток
git branch readme - создаем новую ветку
git branch -D readme - удаляет ветку
git checkout readme - переходим на новую ветку
git checkout -b new - создаем и сразу переходим на новую ветку
git merge readme - совмещение ветки readme и master (readme можно потом удалить)


git config --global user.name - мое имя (если изменить просто добавить в ковычках новое имя)
git config --global user.name - почта
git remote add origin https://github.com/VasilyProfWork/git-course.git - эта команда устанавливает соединение локального репозитория с github
git push -u origin master - заливаем всей файлы на гитхаб

Дальше просто можем делать так 
git status
git add .
git push - заливаем все изменения на гитхаб
git pull - получаем все изменения перед началом работы

git clone https://github.com/VasilyProfWork/git-course.git - добовляем к себе в папку репозиторий (обязательно добовляем в конце .git) 

файл .gitignore нужен для того чтобы в гит не попадали файлы и папки которые мы не хотим отправлять, перечисляем файлы через клавишу enter






