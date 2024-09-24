# Инструкция для работы с Git и удаленнымими репозиториями

## Что такое Git?
Git — один из видов систем контроля версий (или СКВ). Такие системы записывают изменения в набор файлов, а позже позволяют вернуться к определенной версии.

## Принципы работы с Git
У проектных файлов в Git есть 3 базовых состояния

* Измененные (modified) — файлы в процессе рабочего редактирования.
* Индексированные (staged) — та часть измененных файлов, которая уже подготовлена к фиксации после редактирования.
* Зафиксированные (committed) — файлы, уже сохраненные в локальном репозитории.

У Git есть рабочий каталог, где хранятся метаданные и локальная база рабочего проекта. Именно эта часть копируется, когда вы **клонируете** проект (репозиторий) с сервера.

Чаще всего работа с Git устроена примерно так:
1. Вы вносите правки в файлы рабочей копии проекта.
2. Индексируете их, подготавливая к коммиту (здесь Git создает снимки новых правок).
3. Делаете коммит, и индексированные правки наконец сохраняются в вашем каталоге Git.

## Установка Git
Создать свой проект и начать пользоваться Git в нем достаточно просто. Мы будем рассматривать работу в командной строке терминала, потому что там реализован полный набор команд. Вероятно, в будущем вам будет проще воспользоваться встроенными инструментами в крупном приложении (например, в Visual Studio, если вы программист).

Новейшая сборка доступна на официальном сайте Git по [ссылке.](https://git-scm.com/download/win)

## Настройка Git
Самый удобный способ изменения конфигурации — встроенная утилита ***git config***. 

Если запускать ***git config*** без параметров, будет использоваться локальный уровень, никакие из более глобальных настроек не изменятся.

Всю используемую конфигурацию можно просмотреть так:
```> git config --list --show-origin```

Представимся Git, чтобы в рабочих коммитах сохранялось ваше авторство:
```> git config --global user.name "Danil Z"```
```> git config --global user.email danilz@danilz.com```

## Вставка изображения
Чтобы вставить изображение в текст, необоходимо в строчку кода добавить следующее:
![Изображение с названием icon.png](icon.png)

## Блок с конфликтом
Запись до слияния веток
Здесь находится запись **ПОСЛЕ** слияния веток.

## Блок 3 ветки
Тут находится текст, входящий в блок третьей ветки.

### Блок 4 ветки
А здесь находится текст, входящий в блок четвертой ветки.