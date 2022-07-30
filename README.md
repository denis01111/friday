# Обучение Git
![Git logo](git.png)
## Подготовка

Очень важно, создавая **репозиторий**, не иметь **кириллицу** в пути к папке **репозитория**
Также перед началом работы с репозиторием необходимо написать две комманды в терминал:

git config --global user.name «**name**» где **name** - ваше имя английскими буквами

и git config --global user.email *mail@example.com* где *mail@example.com* - ваша почта

Итак, написав эти команды и открыв в ***Visual Studio*** папку, где будет храниться *репозиторий*, необходимо создать файл с расширением **.md** и написать команду ***git init***, что позволит инициализировать *репозиторий*

## Работа с репозиторием

Как только вы закончите работать с файлом, сохраните его комбинаций клавиш ***ctrl + s***

После этого добавьте этот файл в коммит командой ***git add file.md*** где ***file*** - название вашего файла

Если в вашем проекте присутствуют **изображения**, их файлы тоже нужно добавить в *коммит*

Чтобы сделать коммит, напишите команду **git commit** *-m "message"* где *-m "message"* - комментарий к коммиту, его не обязательно писать, но он позволит вам и вашим напарникам легче понять, что за изменения были произведены

Команда ***git status*** позволит получить информацию о текущем состоянии репозитория

С помощью команды ***git log*** можно узнать историю *коммитов* и их *коды*

Команда *git checkout* **0000** где **0000** - первые четыре цифры кода *коммита*, позволяет переходить от одного *коммита* к другому

***git checkout master*** позволяет вернуться к актуальному состоянию файла

***git diff*** показывает разницу между **текущим** файлом и **последнем закоммиченным** файлом

## Обучение Веткам

Чтобы создать новую ***ветку***, вернитесь к актуальному состоянию файла и напишите *git branch* **branch_name** где **branch_name** - название ветки

Чтобы удалить ветку, напишите ***git branch -d branch_name***

Чтобы объединить *ветки*, вернитесь к актуальному состоянию файла и напишите *git merge branch_name*

В случае *конфликтов*, программа позволит вам выбрать, версию файла какой *ветки* использовать, а также позволит сравнить версии между собой

Чтобы перейти на другую ветку, напишите ***git checkout branch_name***

## Гиперссылки

Для того чтобы вставить [гиперссылку](https://gb.ru/), напишите сообщение в квадратных скобках, а затем вставьте нужную вам ссылку в обычных скобках