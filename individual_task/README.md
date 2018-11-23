# Платежная система
## Задание
Разработать приложение-клиент и приложение-сервер платежной системы. 
Участники платежной системы имеют электронные кошельки. 
Электронный кошелек имеет уникальный номер. При регистрации
пользователя в платежной системе на его счет зачисляется определенная
сумма. Пользователя платежной системы могут осуществлять платежи
друг другу через приложение–сервер.

## Клиент
Команды, доступные в клиенте:
- ```REG <login> <password>``` - зарегистрировать нового клиента. После регистрации сервер автоматически залогинит
пользователя в созданном аккаунте.
- ```LOGIN <login> <password>``` - войти в аккаунт.
- ```GET``` - получить состояние счета клиента. Доступно только после входа в аккаунт.
- ```SEND <login> <amount>``` - переслать заданную сумму пользователю с указанным логином. Еще не реализовано
- ```DEL``` - удалить аккаунт.
- ```QUIT``` - выйти из приложения. 

## Сервер
Сервер прослушивает порт 5001. Логи выводятся на консоль и в файл server.log.

Данные пользователей хранятся в автоматически создаваемой папке build/data.