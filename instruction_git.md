## Cоздать новый репозиторий Git.

Для того чтобы создать новый репозиторий используется команда

    git init

С её помощью можно преобразовать существующий проект без управления версиями в репозиторий Git или инициализировать новый пустой репозиторий.
Большинство остальных команд Git невозможно использовать без инициализации репозитория, поэтому данная команда обычно выполняется первой в рамках нового проекта.

*но я, зачем то написал, её в старом(((*

## Отобразить текущее состояние работы Git.

Данная команда отображает состояние рабочего каталога и раздела проиндексированных файлов. С ее помощью можно проверить индексацию изменений и увидеть файлы, которые не отслеживаются Git.

*Проверил ещё раз эту команду, на всякий случай*

    git status

## Добавить изменение рабочего каталога.

Чтобы добавить изменение рабочего каталога в раздел проиндексированных файлов нужно выплонить команду

    git add

Она сообщает Git, что вы хотите включить изменения в конкретном файле в следующий коммит. Однако на самом деле команда git add не оказывает существенного влияния на репозиторий. Изменения регистрируются в нем только после выполнения следующей команды.

## Записать индексированные изменеия в репозиторий.

Это команда Git для записи индексированных изменений в репозиторий. Используется как метка для обозначения всех вопросов, связанных с созданием, редактированием и внутренней структурой коммитов в Git. Прежде чем создавать очередной коммиит, необходимо проиндексировать файлы в рабочей области с помощью команды git aff.

    git commit

## Создать коммит с указаныым комментарием.

Быстрая команда, которая создает коммит с указанным комментарием. По умолчанию git commit открывает локально настроенный текстовый редактор с предложением ввести комментарий к коммиту. При реедаче параметра -m текстовый редактор не открывается, а используется подставленный комментарий.

    git commit -m "message"

## Выполнить коммит состояния со всеми изменениями в рабочем каталоге.

Эта команда включает только изменения отследиваемых файлов, которые были в какой-то момент добавлены в историю с помощью команды git add.

    git commit -a

## Создать коммит всех изменений.
Команда с параметрами -a и -m
Эта комбинация параметров создает коммит всех проиндексированных изменений и добавляет к коммиту подставленный комментарий.

    git commit -am

## Отобразить изменения.

Данная команда отображает отправленные снимки состояния и позволяет просматривать и фильтровать имторию проекта, а также искать в ней конкретные изменения. С помощью git status можно просматривать рабочий каталог и раздел проиндексированных файлов, в то время как данная команда показывает только историю коммитов.

    git log

## Показать коммиты.

Данная команда покажет все ваши коммиты только с первой частью хэша и сообщением фиксации. Каждая фиксация будет находиться в одной строке, как oneline флаг oneline. Опция online печатает каждую фиксацию в одной строке, что полезно, если вы смотрите на множество коммитов.

    git log --oneline

## Отображение истории коммитов.

Для просмотра истории по всем веткам используются флаг --all.

    git log --all

## Я не понимаю данную команду
    git --all --oneline

## Вычисление разницы git деревьев.

Данная команда используется для вычисления разницы между любыми двумя Git деревьями. Это может быть разница между рабочей директорией и индексом

    git diff

## Pазница между индексом и последним коммитом

    git diff --staged
или между любыми двумя коммитами

    git diff master branch

## Переключение между версиями
Это подразумевает переключение между различными версиями целевого объекта. Команда

    git checkout
работает с тремя различными объектами: Файлами, коммитами и ветками. Под переключением также обычно понимают ддействие связанное с выполнением данной команды.

## Ветвление в Git

### Просмотр всех веток

Чтобы посмотреть какие есть ветки в репозитории нужно ввести команду:

    git branch

## Заголовой удаления ветки

### Добавление веток

Чтобы добавить ветку нужно ввести команду:

    git branch <branch_name>

где <branch_name> - имя новой переменной

## Удаленные репозитории

Строка с информацией