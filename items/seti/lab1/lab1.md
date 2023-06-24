# Лабораторная работа №1. Общий доступ к папке

## Краткое описание

В зависимости от используемых ОС хоста и ВМ, потребуется от 2 до 16 ГБ оперативной памяти, не менее 5 ГБ свободного места на диске, наличие интернет-соединения для установки ПО и как минимум 2-х ядерный 64-битный процессор. Работоспособность инструкции проверена на Intel Atom® X5-Z8350 с 4 ГБ ОЗУ.
- На физическом персональном компьютере (хост) с поддержкой технологии виртуализации устанавливается программное обеспечение для эмуляции виртуальных ПК (ВМ)
- Создаются две ВМ в общей подсети - на Linux и Windows
- Обеспечивается наличие двусторонней сетевой связи между ВМ с промежуточным контролем состояния таблиц протокола ARP
- На ВМ с Windows открывается общий доступ к папке
- На ВМ с Linux осуществляется подключение к общей папке
- Осуществляется освобождение занятых ранее ресурсов

### Файлы к лабораторной работе

- [Команды сетевого администрирования и ход выполнения работы (.pdf)](https://drive.google.com/file/d/19VARWEkM4UZvNtEkh5DMrZ6sIZnKO7cQ/view?usp=sharing)
- [Пример отчёта, команды сетевого администрирования и контрольные вопросы (.docx)](https://docs.google.com/document/d/1F6Etb0Tz_e97DiI8sAJQLWIY94FJE_0J/edit?usp=sharing&ouid=114433453162808919564&rtpof=true&sd=true) (Отчёт является неполным и утратил свою актуальность в связи с устареванием использованных дистрибутивов ОС)
- [Подключение общей папки в ОС Linux (.docx)](https://docs.google.com/document/d/1WsI6fw4toooOglIjnDKWdRo6CK807ivW/edit?usp=share_link&ouid=114433453162808919564&rtpof=true&sd=true)

### Контрольные вопросы

- [Версия ответов на контрольные вопросы, составленная коллективно (.docx)](https://1drv.ms/w/s!ArCbKR7X-Y2Ojm7GIoYV9W6BgzcC?e=Qfmn6f) (Доступна для редактирования - улучшения приветствуются)
- [Версия ответов на контрольные вопросы, составленная автором ремейка статьи (.docx)](https://1drv.ms/w/s!AkmVJ_yUg2QsftlyCRT2dOhgmYI?e=WaCEKw) (До 13 вопроса включительно. Возможно, впоследствии я её допишу)

## Подготовка - загрузка необходимых файлов

Для выполнения лабораторной работы потребуются:

- [Visual C++ Redistributable](https://github.com/abbodi1406/vcredist/releases)
- [Oracle VM VirtualBox](https://www.virtualbox.org/wiki/Downloads)
- [Oracle VM VirtualBox Extension Pack](https://www.virtualbox.org/wiki/Downloads)
- Windows XP или выше
- [Alpine Linux](https://www.alpinelinux.org/downloads/) (Версия Virtual x86_64)

### Visual C++ Redistributable

[Загрузка Visual C++ Redistributable](https://github.com/abbodi1406/vcredist/releases)

![Download Visual C++ Redistributable](https://i.imgur.com/JL0TTcQ.png)

### Oracle VM VirtualBox и Oracle VM VirtualBox Extension Pack

[Загрузка Oracle VM VirtualBox и Oracle VM VirtualBox Extension Pack](https://www.virtualbox.org/wiki/Downloads) (Версия Windows hosts для хоста с Windows, остальные - соответственно. Extension Pack - All supported platforms)

![Download Oracle VM VirtualBox and Oracle VM VirtualBox Extension Pack](https://i.imgur.com/G71ZEU9.png)

### Alpine Linux

[Загрузка Alpine Linux](https://www.alpinelinux.org/downloads/) (Версия Virtual x86_64)

![Download Alpine Linux](https://i.imgur.com/H1rqAUy.png)

## Выполнение лабораторной работы

### Создание, настройка и установка виртуальных машин

В моём случае интерфейс менеджера Oracle VM VirtualBox настроен на отображение настроек сети, снимков и экспертного режима. Плагин Oracle VM VirtualBox Extension Pack был предварительно установлен через меню плагинов (также возможна установка и из файлового менеджера. Чтобы кнопка "Установить" стала активной, необходимо пролистать лицензионное соглашение до конца - кто будет делать чистую установку, поделитесь потом скриншотом).

![Tools Network](https://i.imgur.com/BYX3JXm.png)
![VM Snapshots](https://i.imgur.com/FJIsuN9.png)
![Expert mode](https://i.imgur.com/FejQazL.png)

#### Windows XP

Через меню "Машина" -> "Создать" вызываем окно создания ВМ. Данные заполняются, как показано на скриншотах, всё остальное остаётся по-умолчанию. Пути к папке ВМ и образу ISO будут отличаться. Объём жёсткого диска можно уменьшить до 2-5 ГБ.

![Windows XP Name and OS type](https://i.imgur.com/mOeNarZ.png)
![Windows XP Hardware](https://i.imgur.com/3n03WZf.png)

#### Alpine Linux

### Предоставление общего доступа к папке

### Подключение к общей папке
