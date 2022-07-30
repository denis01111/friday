# Обучение Markdown
![Markdown logo](markdown.png)
## Чтобы делать заголовки, добавьте несколько решеток в зависимости от уровня заголовка (1 решетка - заголовок ***первого*** уровня, 2 решетки - заголовок ***второго*** уровня и так далее) и пробел в начале строки

Чтобы писать *курсивом*, добавьте звездочку в начале и в конце текста

Чтобы писать **жирным шрифтом**, добавьте две звездочки в начале и в конце текста

Чтобы писать ***жирным курсивным шрифтом***, добавьте три звездочки в начале и в конце текста

Чтобы писать ~~перечеркнутым шрифтом~~, добавьте две тильды в начале и в конце текста

## Списки

* чтобы сделать такой *список*
* добавьте ***звездочку и пробел***
* в начале строки

1. чтобы сделать такой *список*
2. добавьте ***цифру,*** **точку** и *пробел*
3. в начале строки
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

## Обучение GitHub

![GitHub logo](github.png)

Чтобы начать работать с GitHub, необходимо на нем зарегистрироваться и создать репозиторий. Если вы будете клонировать локальный репозиторий, то можно не создавать файл README.md

Чтобы указать, в какой удаленный репозиторий мы будем вносить изменения, нужно написать команду ***git remote add origin*** *ссылка на удаленный репозиторий*

Чтобы отправить измененный файл в удаленный репозиторий, необходимо написать *git push*

Чтобы получить актуальную версию файла из удаленного репозитория, необходимо написать *git pull*

Чтобы вносить изменение в чужой репозиторий, необходимо сделать его fork на *GitHub* и написать комманду **git clone** *ссылка на fork репозитория*

Чтобы предложить свои изменения для чужого репозитория, после того как вы пушнули ваши изменения нужно на *GitHub* сделать **Pull request**. Желательно при этом указать, какие именно изменения вы сделали, так автору будет легче разобраться
