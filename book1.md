# Библиотека начинающего разработчика

Этот проект содержит справочники по работе в программах, обяательных для старта обучения программированию.

****

## Разделы справочника

1. Синтаксис языка Markdown

   1.1 Общие сведения о Markdown

   1.2 Основные элементы Markdown

2. Инструкции для работы в Git

   2.1 Общие сведения о программе Git

   2.2 Горячие команды программы Git

3. Инструкции для работы в GitHub

****

## 1. Синтаксис языка Markdown

### 1.1 Общие сведения о Markdown

Markdown — язык текстовой разметки. Он предназначен для создания текстов в обычных файлах формата TXT с жирным или курсивным начертанием, цитатами, ссылками и даже таблицами. Достаточно запомнить простые правила Markdown, и можно писать хоть в «Блокноте».

Этот язык разметки совместим с многими онлайн-редакторами и блог-платформами. Можно написать черновик для своего блога в Markdown, а потом опубликовать его за секунды — все ссылки, заголовки и форматирование будут выглядеть так, как и задумывалось.

Документы Markdown легко экспортировать в любые форматы: PDF, DOC, ODT. При этом их форматирование остаётся неизменным.

Тексты в Markdown оформляются посредством специальных символов, вставляемых перед или после слов и фраз. Вот самые простые правила, которые работают во всех редакторах.

### 1.2 Основные элементы Markdown

- символ # (решётка, хеш). Уровень заголовка определяется количеством решёток в нём, всего их может быть шесть;

- форматирование текста можно сделать курсивным или жирным при помощи звёздочек и подчёркиваний;

- если какой-то абзац нужно выделить как цитату необходимо проставлять перед каждой строчкой цитаты использовать знак >;

- списки маркированные списки делаются с помощью дефиса, проставляемого перед каждым пунктом, нумерованные с ипользованием цифр;

- горизонтальная линия вставится в документ если три раза (или больше) использовать один из этих символов на клавиатуре: *, — или _, и   . Если строкой выше над ней стоит ещё какой-то текст, он станет заголовком первого уровня. Линию можно использовать, чтобы разделять большие главы документа;

- изображение вставится если поставить восклицательный знак, подпись к изображению в квадратных скобках и ссылку на него в круглых скобках. Можно указывать ссылки на картинки как из интернета, так и на хранящиеся на жёстком диске. Подпись указывать необязательно.

****

## 2. Инструкции для работы в Git

### 2.1 Общие сведения о программе Git

#### Что такое Git?

*Git - это одна из реализаций распределённых систем контроля версий, имеющая как и локальные, так и удалённые репозитории. Является самой популярной реализацией систем контроля версий в мире.*

#### Глобальные начальные инструкции

*Перед первичным запуском работы с проектами пользователю необходимо ввести данные своего имени и электронной почты командами:*

git config --global user.name "<имя>"

git config --global user.email "<почта_@_>"

*В дальнейшем указанные данные будут прописываться в шапке документов Git.*

#### Подготовка репозитория

*Свои файлы система Git сохраняет в репозитории - папке с расширением  . git, имеющей скрытый формат.  Указанная папка создается на желаемом уровне отслеживания рабочих папок и файлов. Папку можно увидеть если настроить отображение скрытых папок на компьютере. Для создания папки-репозитория   необходимо  выполнить команду "git init", указав путь к ней.*

#### Принцип работы Git

*Система Git архивирует данные о рабочем файле в созданной папке-репозитории путем командного обращения к ней с инструкциями изначально добавить один (или несколько файлов) (командой "git add "). В папке - репозитории Git создает много разных папок, в которых сохраняет и полную копию файла (перезаписывает на последний сохраненный вариант, в случае если были изменения в файле), фиксирует изменения между этим состоянием и ранее зафиксированным состоянием, присваивает данному состоянию уникальный код в виде хеш - строки из 40 символов букв и цифр (хеша), сохраняет данные о контрольной сумме. Если в файле произошли изменения, то это отражается на контрольной сумме и файл считается измененным. Пользователь принимает самостоятельное решение в какой момент времени он желает заархивировать сохранить текущий вариант своего рабочего файла, чтобы иметь возможность воспользоваться им в дальнейшем в случае необходимости.*

****

### 2.2 Горячие команды программы Git

- git init - *стартовая команда cоздания папки-репозитория в папке рабочего (контролируемого) файла*:

*Синтаксис:*

git init

- git status - *выводит данные о текущем состоянии рабочего файла*

*Синтаксис:*

git status

- git diff - *позволяет сравнить текущие изменения в рабочем файле с его последним сохраненным вариантом*:

*Синтаксис:*

git diff

- git add - *выполняет задачи начала архивирования состояния рабочего  файла на момент его последнего сохранения (Сtrl+S), производит индексацию этого состояния в репозитории*:

*Синтаксис:*

git add  <имя файла> - *индексирует конкретный файл*;

git add . - *индексирует все файлы рабочей папки*;

- git commit - *завершает задачу сохранения проиндексированного командой*  add  *зафиксированного состояния файла*;

*Синтаксис:*

git commit -m "<комментарий> " - *архивирует данные о состоянии файла с комментарием пользователя*;

- git log - *выводит список зафиксированных именений файла*:

*Синтаксис:*

git log -*выводит полный список информации о фиксированных состояниях в виде хэш-строк, комментариев к коммитам, авторе, дате с времени изменения*;

git log --graph - *создает графическое представление структуры коммитов в ветке*;

- git branch - *работает с ветками: показывает текущую , создает новую или удаляет ненужную нетекущую*:

*Синтаксис:*

git branch - *выводит список веток и выделяет текущую*;

git branch <имя ветки> - *создает новую ветку*;

git branch -d <имя ветки> - *удаляет требуемую неактивную ветку*;

- git checkout - *работает с ветками*:

*Синтаксис:*

git checkout <имя ветки> - *делает указанную ветку текущей*;

git checkout main - *делает главную ветку текущей*;

git checkout -b <имя ветки>- *создает новую ветку и делает ее текущей*

## GitHub

GitHub — это популярный сайт, где можно хранить репозитории и работать с ними. Ещё это крупнейшая площадка, где разработчики размещают проекты с открытым исходным кодом.
GitHub предоставляет функции для управления системой контроля версий кода, общения с другими разработчиками, просмотра репозиториев других разработчиков, контроля доступа, багтрекинга, управления задачами, ведения истории коммитов, интеграции с другими сервисами, ведения документации.

## Как создать проект на GitHub

Чтобы выложить на сайт GitHub проект нужно пройти регистрацию:

1. Указать адрес электронной почты (он же станет логином для учётной записи);
2. Указать НИК пользователя.

## Начало работы в аккаунте в GitHub

После регистрации открывается панель управления, где будет отображаться статистика и созданные репозитории.

### Репозитории  в GitHub

Репозиторий в GitHub может быть:

* приватный - репозиторий, к которому может подключится ограниченное число человек;
* публичный - репозиторий, неимеющий ограницений на число участников проекта.

Репозитории могут включать файл README с информацией о проекте.

### Создание репозитория

Чтобы создать репозиторий необходимо воспользоваться  выпадающим меню в правом верхнем углу на любой из страниц GitHub. Можно создать новый или загрузить имеющийся на локальном компьютере. GitHub отобразит подсказку, как создать или импортировать репозиторий.

Чтобы загрузить репозиторий с другого аккаунта нужно со страницы своего акунта зайти через поле поиска репозиториев, расположенного в левом верхнем углу. Когда поиск будет произведен аккаунт друга ( коллеги, и др) дудет открыт и станет доступной кнопка Fork, после чего будет открыто окно для ввода имени для собственного репозитория. Далее просто нажать кнопку "Создать".

Затем берем сслку на адрес созданного репозитория и на своем локальбном компьютере делаем операцию клонирования в заранее подготовленную папку и переводим  в нее фокус директории.

Добавляем файлы для отслеживания, делаем коммит

Создаем новую ветку и вносим изменения в файл
Фиксируем изменения и отправляем версию файла в свой аккаунт, находясь не на главной ветке

Если все готово для отправки пулла хозяину реппозитория, то делаем Пулл-реквест из второстепенной ветки

Далее изменения будут рассмотрены хозяином и приняты или нет, ответ придет на эл. почту.
