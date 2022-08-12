# infotecs-tests
Проект с тестами для первого задания.
Для подтягивания зависимостей использовался Maven.
Jar-файл собирался с помощью Intellij Idea.

Чтобы запустить тесты, нужно просто запустить tests.jar

# Обоснование тестов

## TestStudent

Нужно проверить корректнось работы get методов, действительно ли они возвращают те значение, которые были переданы конструктору, т.к. в дальнейшем эти методы будут использоваться для нужных студентов в списке

## TestCommandManager
Нужно проверить, правильно ли работает метод, который обновляет данные на сервере при выполнении некоторых команд
Проверяем сценарии позитивный сценарий, когда у нас есть установленное соединение с сервером.
А также сценарий, когда соединения нет.
В обоих случаях метод должен отправить данные на сервер, т.к. при отстутствии соединения, внутри метода мы пытаемся подключится к сеерверу заново.

## TestCommands
Проверяем работу команд. Для каждой команды проверяем ситуацию когда она выполнилась успешно и когда она не смогла выполнить заданное действие.

## TestFTPConnection
Проверяем как ведет себя программа при установлении соединения с сервером. Рассматривается позитивный сценарий и 2 негативных, когда мы либо не смогли подключится к серверу, либо ошиблись в логине или пароле.

