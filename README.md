# *Шпаргалка Git для друга* 

Здесь ты найдешь полезные команды и советы для работы на Git

---

## *Базовые команды в консоли* 

Навигация

pwd```bash (от англ. print working directory, «показать рабочую папку») — покажи, в какой я папке;

ls```bash (от англ. list directory contents, «отобразить содержимое директории») — покажи файлы и папки в текущей папке;

ls -a```bash — покажи также скрытые файлы и папки, названия которых начинаются с символа .;

cd first-project```bash (от англ. change directory, «сменить директорию») — перейди в папку first-project;

cd first-project/html```bash — перейди в папку html, которая находится в папке first-project;

cd ..```bash — перейди на уровень выше, в родительскую папку;

cd ~```bash — перейди в домашнюю директорию (/Users/Username);

cd /```bash — перейди в корневую директорию.

### *Работа с файлами и папками*

Создание

touch index.html```bash (англ. touch, «коснуться») — создай файл index.html в текущей папке;

touch index.html style.css script.js```bash — если нужно создать сразу несколько файлов, можно напечатать их имена в одну строку через пробел;

mkdir second-project```bash (от англ. make directory, «создать директорию») — создай папку с именем second-project в текущей папке.

Копирование и перемещение

cp file.txt ~/my-dir```bash (от англ. copy, «копировать») — скопируй файл в другое место;

mv file.txt ~/my-dir```bash (от англ. move, «переместить») — перемести файл или папку в другое место.

Чтение

cat file.txt```bash (от англ. concatenate and print, «объединить и распечатать») — распечатай содержимое текстового файла file.txt.

Удаление

rm about.html```bash (от англ. remove, «удалить») — удали файл about.html;

rmdir images```bash (от англ. remove directory, «удалить директорию») — удали папку images;

rm -r second-project```bash (от англ. remove, «удалить» + recursive, «рекурсивный») — удали папку second-project и всё, что она содержит.

---

#### *Статусы файлов в Git*
    Статусом untracked помечается файл, о существовании которого Git знает, но не следит за изменениями в нём. Этот статус — противоположность tracked, в который попадают все файлы, отслеживаемые Git.
    Файл переходит в статус staged после выполнения git add.
    Статус modified означает, что файл был изменён.
    Большинство файлов в проектах «шагает» по следующему циклу: «изменён» → «добавлен в список на коммит» → «закоммичен» → «изменён» → и так далее.

---

##### *HEAD — всему голова*

Папка .git содержит много непонятных файлов — об одном из них мы рассказали в этом уроке. Подытожим:

    В числе прочих файлов в папке .git есть служебный файл HEAD. Он указывает на самый свежий коммит.
    Вместо хеша последнего коммита можно написать слово HEAD — Git вас поймёт.

---





