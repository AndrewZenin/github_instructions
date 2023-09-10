Я - очень длинный файл. Сократите меня. И пусть в живых из двух файлов останется только один. Таков путь!
83 миллиона пользователей, четыре миллиона организаций и 200 миллионов репозиториев. В Сети много сервисов для размещения исходного кода своих проектов, но говорят чаще всего именно про GitHub. В чём же дело?

Конечно, известный владелец сервиса (Microsoft) и привычка играют свою роль, но главная причина — возможности платформы.

Что такое GitHub и чем он отличается от Git

Как понять, нужен ли вам GitHub

Основные концепции GitHub простыми словами

Создание репозитория и загрузка файлов

Просмотр файлов в репозитории

Поиск и чтение репозиториев

Создание веток

Переключение веток и решение конфликтов

Настройка описания репозитория

Создание сайта из вашего GitHub-профиля

Подключение GUI-клиента GitHub Desktop

Работа с GitHub через CLI

Настройка GitHub-профиля

Вместо end()

Что такое GitHub и чем он отличается от Git
GitHub — это облачная платформа для хостинга IT-проектов и совместной разработки, под капотом которой находится популярная система контроля версий Git, а также полноценная социальная сеть для разработчиков.

Здесь можно найти кучу open-source-проектов на разных языках и поучаствовать в них, разместить своё портфолио с примерами кода, чтобы приложить ссылку к резюме, подглядывать в открытых проектах интересные архитектурные решения, смотреть, как опытные разработчики пишут код, и скачивать огромное количество полезных в разработке и бесплатных инструментов для разработки. Кстати, некоторые умельцы умудряются собирать в GitHub целые библиотеки — книг и статей, а не программистские либы :)

И да, если вы недовольны какими-то фичами в любимой открытой программе и она выложена на GitHub, вы всегда можете прийти и поругаться в комментариях к проекту :) А лучше всего — оформить issue (мы расскажем, что это) и самостоятельно пофиксить проблему на радость всем пользователям. Не забывайте и благодарить авторов классных открытых проектов — донатами и просто тёплыми словами. Им будет очень приятно.

Придя практически в любую IT-компанию, вы столкнётесь с тем, что код где-то хранится — и в подавляющем большинстве случаев этим «где-то» будет именно GitHub. У GitHub есть довольно известный конкурент — GitLab, он тоже основан на Git, но это разные платформы разных компаний, хотя их функциональность очень похожа.

А ещё не стоит путать GitHub и Git. GitHub — лишь одна из реализаций системы контроля версий Git (только взгляните на полный список Git-клиентов с графическим интерфейсом), в которую добавлено много удобных инструментов и возможностей (те же комментарии, issues, гиперссылки, форматированный текст и тому подобное). Помните, GitHub можно использовать и без знания Git (обратное тоже верно).

Ну как, звучит круто? Тогда приступайте к нашему гайду о том, как пользоваться GitHub, чтобы во всём разобраться и вообще понять, нужен ли он вам прямо сейчас.

Как понять, нужен ли вам GitHub
Безусловно, GitHub нужен не всем. Допустим, вы ещё только учитесь кодить или неспешно делаете небольшой проект для личного пользования — и вас устраивает хранение проекта на локальной машине. Может, сейчас вы просто учите язык, который вам нравится, и на данном этапе не хотите хвататься за всё сразу.

В первую очередь GitHub необходим проектам с частыми обновлениями, множеством версий, большим количеством файлов, необходимостью синхронизации разработки и удобного развёртывания.

И действительно, есть множество других способов хранения исходников: можно создать для них папку в разделе «Мои документы», закидывать их в облако и подписывать версии или даже загружать в «Избранное» в Telegram или «ВКонтакте» (костыльно, да, но вполне реально).

А ещё можно накидывать список изменений в заметках в телефоне/на холодильнике текстом в приватном Telegram-канале. Можно деплоить проект с помощью простого скачивания и распаковки ZIP-архива с файлами вашей программы (особенно если цель — просто показать программу другу или девушке, которой вы пришли «помочь с ноутбуком» ^_^). В конце концов, можно сообщать о багах в вашем любимом фреймворке сообществу анонимов в паблике в VK — возмущаться вместе очень весело.

Все эти способы по-своему хороши, но для работы в IT нужно привыкать к GitHub: это стандарт индустрии.

Интересный факт: недавно появилась российская альтернатива GitHub под названием GitFlic. Команда сервиса заявила, что намерена дать «новый импульс разработке отечественных операционных систем, программ, приложений и серверных решений». Среди цепляющих возможностей — интеграция с Telegram.

Большая часть необходимых возможностей GitHub бесплатна, хотя у платформы есть и платные тарифы — однако с ними можно долго не сталкиваться, потому что бесплатных обычному разработчику хватает с лихвой.



Это Фрай. Он не смог использовать GitHub и улетел в будущее. Не будьте как Фрай_Кадр: мультсериал «Футурама»_

Основные концепции GitHub простыми словами
Новичков интерфейс GitHub может сбивать с толку: за годы с момента создания площадка обросла множеством инструментов, но главное остаётся неизменным.

Почти вся терминология наследуется у Git. Основные термины — репозиторий, ветка, коммит, форк. Выбор некоторых из этих названий может показаться не очень интуитивным (даже если вы владеете английским), но так уж сложилось.

Как заливать файлы, создавать репозитории и проводить другие операции, мы рассмотрим в следующем разделе, так что не пугайтесь упоминания разных действий в определениях терминов — всё покажем с картинками :)

Репозиторий
Это просто корневая папка с файлами и вложенными директориями вашей программы — и одновременно её страница на GitHub. Загрузить в репозиторий можно всё что угодно, но предполагается, что вы будете хранить в нём файлы с исходным кодом и какие-нибудь дополнительные материалы — допустим, необходимую для GUI или вёрстки графику (картинки, иконки и тому подобное).

Репозитории могут быть публичными и приватными, в них можно создавать другие папки и отслеживать изменения версий. Управлять своими репозиториями можно прямо через интерфейс сайта, командную строку, десктопное приложение GitHub или различные средства разработки (IDE), поддерживающие интеграцию с сервисом.



Ветка (branch)
В ветки группируются изменения и обновления — допустим, одна главная ветка (по умолчанию создаётся main) и одна beta. Ветки независимы друг от друга, но при желании их можно объединять (merge — слияние) — даже если между ними есть разница в коде.

Способы изменения репозитория: коммит, пуш, клон, форк
Внести в содержимое репозитория изменения можно напрямую или создав копию. Само внесение изменений называется «коммит» (от английского commit — совершить), у него есть временная метка и хеш-сумма.

Перенос изменений-коммитов из локального репозитория (на вашем ПК) на удалённый (remote repository, то есть в данном случае на GitHub) называется «пуш» (push) — от английского «толкать» (дословно — «проталкивать» изменения).

Скопировать репозиторий для внесения изменений в копию можно двумя основными способами:

клонировать (clone) — то есть просто скопировать на локальный компьютер или сервер;
или форкнуть (от английского fork — развилка) — сделать отдельную копию репозитория (обычно чужого) для продолжения разработки «по другому пути развилки».
Если вы форкнули чужой проект, чтобы предложить автору конкретные улучшения, нужно по готовности «запулить» их в исходный репозиторий — то есть сделав pull request (запрос на изменения).

Это 90% необходимых фактов. Более скучные подробности описаны в документации и разделе обучения GitHub, а также в руководстве по самому Git, ну а мы попробуем применить всё это на практике.

Создание репозитория и загрузка файлов
Конечно, самый простой способ пользоваться GitHub — через сайт, поэтому начнём отсюда.

Самые типичные действия при работе с репозиторием — его создание и загрузка файлов, их мы уже рассматривали ранее. Легко убедиться, что обе задачи занимают не больше 30 секунд.

Очень кратко повторим выводы из нашего прошлого материала:

для создания репозитория нужно нажать на + в правом верхнем углу сайта, выбрать пункт New Repository, заполнить название и описание, проставить нужные галочки и щёлкнуть на Create Repository;
для загрузки файлов нужно зайти в нужный репозиторий, щёлкнуть на Add file и выбрать Upload files.
12



Шаг 1. Создание GitHub-репозитория в веб-версии_Скриншот: Skillbox Media_



Шаг 2. Страница создания GitHub-репозитория_Скриншот: Skillbox Media_

Но для обучения Тёмной стороне Силы работе с GitHub полезно потренироваться выполнять и другие необходимые в процессе разработки действия: клонирование/форк, объединение веток, просмотр и разрешение конфликтов и другие.

Давайте пошагово пройдём всё это вместе — сначала через сайт, а потом взглянем одним глазком на работу через GUI-клиенты и интерфейс командной строки (CLI).

Просмотр файлов в репозитории


Выбор файлов в GitHub-репозитории для их просмотра_Скриншот: Skillbox Media_

Согласитесь, что в ряде случаев удобно не скачивать исходники, а просто бегло ознакомиться с ними. Для таких простых операций вовсе не нужен десктопный клиент: все файлы можно быстро открыть в веб-версии (и код, и те же картинки). Просто щёлкните по ним для просмотра!

12



На этой картинке — просмотр файла с кодом. Всё как полагается: есть нумерация строк и подсветка синтаксиса_Скриншот: Skillbox Media_



А здесь — просмотр картинки, которая нужна нам для GUI и потому также залита в репозиторий_Скриншот: Skillbox Media_

Поиск и чтение репозиториев
Хотя сёрфинг по чужим репозиториям — залипательное времяпровождение, в первую очередь это один из способов нахождения полезных инструментов вам в помощь. Над многими функциями, которые вы хотели бы добавить в своё приложение, уже кто-то работал, остаётся только найти GitHub-репозитории таких проектов.

Как и в других случаях поиска, вы можете выйти на нужный репозиторий из поисковика или через внутренний поиск по GitHub.



Для примера: это официальный GitHub-репозиторий Android-приложения Telegram. Смотрим на детали: краткое описание — About (Telegram for Android source), две ветки (там master и dev), в мастере 462 коммита, 227 пул-реквестов, последний релиз шесть дней назад, лицензия GPL 2.0, 1,2 тысячи наблюдателей, 7,1 тысячи форков и целая 21 тысяча добавлений в закладки_Скриншот: Skillbox Media_

Важнее другое — на что обращать внимание. Пройдёмся по некоторым пунктам со скриншота выше.

Во-первых, самое очевидное — это описание на главной странице. Именно в нём находится ответ на ваш главный вопрос — что это и чем может вам помочь.

Если точнее, предусмотрено два описания репозиториев — краткое (один абзац справа вверху) и полное (по центру, под списком файлов).

Если репозиторий кажется полезным, дальше нужно понять, на каких условиях вы можете его использовать, что зависит от указанной автором лицензии.

После этого оцените, подходит ли вам частота обновлений, — это можно сделать в разделе Releases (ссылка прямо под кратким описанием). Конечно, это зависит от ситуации: где-то может пригодиться инструмент, который не обновлялся четыре года, но чаще всего нужна хотя бы минимальная поддержка — то есть обновления минимум раз в несколько месяцев.

Важно знать и где посмотреть количество и содержание коммитов — кликабельный счётчик находится над списком файлов справа.

Наконец, стоит взглянуть и на количество отметок, демонстрирующих популярность проекта среди сообщества, — отслеживаний, форков и звёздочек (это в каком-то смысле местные аналоги лайков и репостов).

Ещё чуть ниже справа — одна из самых интересных штук: анализ используемых в репозитории языков программирования. В репозитории со скриншота выше набор выглядит так.



Языки программирования, на которых написан код загруженных в репозиторий исходников Android-приложения Telegram_Скриншот: Skillbox Media_

Вообще, неплохо изучать репозитории известных приложений, которыми сами пользуетесь (как на скриншоте выше), и отмечать понравившиеся звёздочками. Это не только интересно — со временем GitHub изучит ваши предпочтения и станет предлагать в блоке Explore то, что вам может понравиться.



Пример: GitHub-репозиторий VK_Скриншот: Skillbox Media_

Создание веток


Создаём альтернативную ветку №1 — koshka_Скриншот: Skillbox Media_

Создать новую ветку очень просто:

Жмём на большую зелёную кнопку New branch.
Вводим название новой ветки.
Выбираем исходную ветку для копирования (то есть main, так как пока других и нет).
Щёлкаем на Create branch.
Переключение веток и решение конфликтов
В данном случае нужно сначала уточнить, что имеется в виду: если необходимо просто зайти в альтернативную ветку, это можно сделать в списке веток репозитория (нужная ссылка есть над списком файлов).

Создадим также альтернативную ветку №2 (sava) и посмотрим, как всё это выглядит в итоге.



Список веток репозитория: основная и две альтернативных_Скриншот: Skillbox Media_

Можно говорить и про переключение между ветками в другом смысле — когда изменения из альтернативной ветки сливают с главной веткой. Смотрите: у нас есть файл code.js, но его содержимое немного отличается:

в ветке main там JS-команда console.log («Дефолтная ветка») и картинка с великим маэстро современности Риком Эстли;
однако в ветке koshka тот же файл содержит команду console.log («Кошка!»);, а вместо Рика — смешной кот;
и всё совсем усложняется третьей веткой sava, где консольный вывод вида console.log («Сова!»); и используется картинка с совой (естественно, все перечисленные картинки во всех ветках называются одинаково — pic.jpg).
Получается, между ветками есть конфликт и просто слить любую из альтернативных веток с главной нельзя! Но для этого уже есть решение: GitHub предлагает нам сравнить конфликтующие ветки, и если мы захотим, то и запулить изменения в основную — то есть сделать тот самый pull request, о котором говорилось выше.



Так GitHub сообщает, что в некоторых ветках есть изменения_Скриншот: Skillbox Media_

Вот как выглядит сравнение веток (c koshka и sava соответственно).

12



Сравнение ветки main с веткой koshka_Скриншот: Skillbox Media_



Сравнение ветки main с веткой sava_Скриншот: Skillbox Media_

Допустим, мы решаем принять изменения из ветки sava и создаём pull request с небольшим комментарием.



Создание пул-реквеста для слияния изменений из ветки sava с веткой main_Скриншот: Skillbox Media_

Дальше он появляется в списке пул-реквестов репозитория, где мы определяем дальнейшую судьбу данного запроса на изменения.



В соответствующем разделе репозитория появился новый пул-реквест_Скриншот: Skillbox Media_

Пул-реквест можно окончательно принять, подтвердив слияние (merge) веток, или отклонить, закрыв запрос (Close pull request).

12



Шаг 1. Рассмотрение пул-реквеста_Скриншот: Skillbox Media_



Шаг 2. Рассмотрение пул-реквеста_Скриншот: Skillbox Media_

При этом главную ветку main можно защитить от изменений, включив соответствующие опции в настройках репозитория (что вам и будет предложено при создании новых веток).



GitHub предлагает защитить ветку от нежелательных изменений_Скриншот: Skillbox Media_

Чтобы поменять данный ряд параметров, зайдите в своём репозитории в раздел Settings -> Branches. Нужные настройки — в подразделе Branch protection rules (целых 10 галочек на выбор).

Настройка описания репозитория
Основное описание вашего GitHub-проекта задаётся в файле Readme.md, который можно создать вместе с репозиторием или после. Расширение md — это просто сокращение от названия популярного языка упрощённой разметки контента — Markdown.

Содержимое файла Readme отображается на главной странице репозитория и отвечает на вопрос, что это за проект, чем он может быть полезен другим разработчикам и как им воспользоваться.

Чтобы оформить Readme со вкусом, можно воспользоваться руководством GitHub по markdown-разметке. Вот как будет выглядеть Readme нашего репозитория-примера после прокачки (первый и второй экран соответственно).

12



Настройка файла Readme GitHub-репозитория_Скриншот: Skillbox Media_



Настройка файла Readme GitHub-репозитория_Скриншот: Skillbox Media_

Обратите внимание: в оформлении можно использовать всё что угодно — заголовки разных уровней, выделение жирным/курсивом, изображения, эмодзи, ссылки и так далее.

Файл Readme может быть довольно длинным, но всё же для оформления большой документации GitHub рекомендует создать «Вики».

Создание сайта из вашего GitHub‑профиля
Захостить сайт на GitHub можно с помощью функции GitHub Pages. Это очень просто:

Зайдите в настройки репозитория.
В блоке Code and automation выберите Pages.
Выберите источник (Deploy from a branch, затем нужную ветку).
Кликните на Save.
Обновите страницу, и вверху страницы появится ссылка на ваш новый сайт.


Пример сайта на GitHub Pages_Скриншот: Skillbox Media_

В случае создания сайта для продвижения себя, а не проекта, просто создайте репозиторий с кодом сайта-визитки и дайте ему имя вида [username].github.io, где username — название вашего аккаунта на GitHub. Более подробно про эту функцию — тут.

Подключение GUI-клиента GitHub Desktop
Если вам удобнее такой способ работы, здесь всё тоже просто. Опять же, повторим кратко выводы из нашего более подробного гайда на эту тему:

Скачиваем и устанавливаем сам клиент.
Авторизуемся в своей учётной записи.
Работаем с существующими репозиториями или создаём новые (локальные).


Главное меню GUI-клиента GitHub Desktop для Windows. Видим в списке и наш репозиторий skillbox_cool, описанный выше_Скриншот: Skillbox Media_

Приложение предлагает выполнить клонирование репозитория на локальную машину для дальнейшей работы, что мы и сделаем.



Клонирование репозитория в десктопном клиенте GitHub_Скриншот: Skillbox Media_

Клонированные из удалённого GitHub-репозитория файлы хранятся в специальной папке на вашем компьютере, и в них легко вносить изменения — клиент будет открывать их в выбранном вами редакторе кода / среде разработки (хотя удобнее всё по отдельности — выбрав нужный файл-исходник в папке).

В общем, всё просто, как раз-два-три.

Работа с GitHub через CLI
Работать с GitHub можно и через командную строку Windows или PowerShell. Это не очень сложно: для начала интерфейс командной строки также нужно скачать и установить (документация — здесь).



Работа с GitHub CLI в PowerShell_Скриншот: Skillbox Media_

Команды для GitHub CLI начинаются с сокращения gh — к примеру gh repo clone.



Интерфейс GUI Git_Скриншот: Skillbox Media_

Есть и другой вариант — использовать собственно Git и работать через его собственный CLI. Git скачивается и устанавливается отдельно, там есть минималистичный GUI, но его уже логичнее использовать в терминале.



Работа с Git CLI в PowerShell_Скриншот: Skillbox Media_

Главное, что нужно про это знать: все команды Git начинаются соответственно — со слова git, после чего указывается тип действия: git clone, git merge, git fork и прочее. Чтобы воспользоваться ими, установите Git, распечатайте себе любую памятку по его командам и смело начинайте ими пользоваться.

Настройка GitHub-профиля
Кастомизация профиля — важная часть самопрезентации разработчика: резюме, визитная карточка и витрина проектов, над которыми вы работали.

Эту информацию оценивают работодатели, поэтому стоит заполнить информацию о себе и сделать публичными несколько ваших лучших репозиториев (конечно, если там ничего секретного :)) — именно они будут частью вашей персональной витрины.

Посмотрим на профиль какого-нибудь крутого разработчика из тех, кто сейчас в тренде GitHub (да-да, есть и такой раздел).



Топ-25 разработчиков по версии GitHub (на момент написания материала)Скриншот: личный архив автора

На первом месте — некий Стивен Селис. А что в его профиле? Указано место работы, есть сайты и контакты, а в статистике — 123 репозитория и 1725 изменений в репозиториях за год (круглый год). То есть невооружённым глазом видно, что человек как минимум активный и опытный.



GitHub-профиль одного из топовых разработчиков (1-е место в рейтинге GitHub на ноябрь 2022 года). Зелёные квадратики — это активность автора_Скриншот: Skillbox Media_

Даже если вы пока ещё не в топе GitHub, нужно стремиться к подобному наполнению профиля: подробная информация + показательный ряд проектов (вы можете закреплять их по-своему, нажав в собственном профиле на Customize your pins).

Вместо end()
Всё не так сложно, как может показаться (говоря иносказательно, каждый разработчик в своей жизни сначала учится есть вилкой, а потом — форкать GitHub-репозитории).

GitHub пользуются все: это один из важных общих навыков вне зависимости от выбранного вами языка программирования и направления разработки. И, как и школьные уроки ОБЖ, тот же git clone когда-нибудь вас спасёт.

Поэтому важно начинать пользоваться GitHub как можно раньше — хотя бы даже для бэкапов учебного кода, и уже скоро это станет полезной привычкой.