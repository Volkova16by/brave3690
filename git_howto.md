# Подсказка по Git


**Введение**

* Git - один из видов систем контроля версий. Такие системы записывают изменения в набор файлов, а позже позволяют вернуться к определенной версии. Вам может пригодится Git, если вы например, программист, системный администратор, дизайнер (или в целом работаете с массивом изеняющихся файлов) и хотите сохранить каждую версию проекта.
Вы сможите вернуться к любому из сохраненных состояний, посмотреть изменения и увидеть их авторов.Так гораздо проще исправить возникающие проблемы.

## Установка Git 

 * Установка Git для Windows, MAC, linux [https://git-scm.com/downloads](https://git-smc.com/downloads "Всплывающая подсказка")

* Чтобы использовать коммиты, нужно представиться Git. Для "авторизации" в Git потребуется ввести имя и почту в терменале VSC(куда мы и вводим команду "git init"). 
>>Для ввода имени используем: git config --global user.name


>>Для ввода почты используем: git config --global user.email



## Создания репозитория

### Основные команды

```sh
git init - 
cоздает новый локальный репозиторий с заданным именем.
```
```sh
git status -
gеречисляет все новые или изменённые файлы, которые нуждаются в фиксации.
```
```sh
git add - 
индексирует указанный файл для последующего коммита.
```
```sh
git commit -m "Message text" -
фиксирует проиндексированные изменения и сохраняет их в историю версий. 
```
```sh
git log -
история коммитов для текущей ветки.
```
```sh
git log --oneline -
вывод коммитов в одну строку. Показывает только хэш коммита и commit message.
```
```sh
git checkout -
переход от одного коммита к другому.
```
```sh
git checkout master -
вернуться к актуальному состоянию и продолжить работу.
```
```sh
git diff -
увидеть разницу между текущим файлом и закоммиченным файлом.
```
Отображение всех веток 
```sh
git branch 
```
Перемещение по веткам


```
git checkout <имя_ветки>

```

Cоздание новой ветки
```sh
git branch <имя ветки>
```
Удалить ветку
```sh
git branch -d <имя ветки>

```
Просмотреть лог коммитов с визуализацией
между ними, создает графический обзор веток
```sh
git log --oneline --graph
```


# Добавим как добвлять картинки в Git

Это собака
![Собака](dog.jpg)

# Работа с удаленными репозиториями

```sh
git fetch
Команда git fetch связывается с удалённым репозиторием и забирает из него все изменения, которых у вас пока нет и сохраняет их локально.
```
```sh
git pull
Команда git pull работает как комбинация команд git fetch и git merge, т. е. Git вначале забирает изменения из указанного удалённого репозитория, а затем пытается слить их с текущей веткой.
```
```sh
git push
Команда git push используется для установления связи с удалённым репозиторием, вычисления локальных изменений отсутствующих в нём, и собственно их передачи в вышеупомянутый репозиторий. Этой команде нужно право на запись в репозиторий, поэтому она использует аутентификацию.
```
```sh
git remote
Команда git remote служит для управления списком удалённых репозиториев. Она позволяет сохранять длинные URL репозиториев в виде понятных коротких строк, например «origin», так что вам не придётся забивать голову всякой ерундой и набирать её каждый раз для связи с сервером. Вы можете использовать несколько удалённых репозиториев для работы и git remote поможет добавлять, изменять и удалять их.
```

**Заключение**

Git *как контентно-адресуемая файловая система - очень мощный инструмент, который можно использовать как нечто большее, чем просто систему контроля версий* Git поможетвам написать своё крутое приложение, использующее эти технологии, и позволит вам чуствовать себя свободнее с Git даже в продвинутых вещах. 