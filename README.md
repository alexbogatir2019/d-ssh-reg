## Задание 1

Подключиться к серверу на [reg.ru](https://www.reg.ru/) с помощью [ssh](https://losst.ru/kak-polzovatsya-ssh).

По шагам:

1. Получить доступ к учетной записи на reg.ru. Для этого нужно перейти по ссылке в личном кабинете Нетологии в разделе занятия "Доступ к VPS от Reg.ru" и зарегистрироваться на сайте. 

2. Установить терминал с ssh-клиентом:

- для ubuntu/fedora/centos/etc. - ssh-клиент уже установлен, ничего делать не надо
- для macOS - ssh-клиент уже установлен, ничего делать не надо
- для windows - рекомендуется установить [wsl 2](https://docs.microsoft.com/ru-ru/windows/wsl/install-win10)

3. Создать сервер в личном кабинете на reg.ru (подробности в [создание сервера на reg.ru](./new-server-reg-ru.md))

4. Узнать IP созданного сервера, логин и пароль пользователя на сервере (в своем личном кабинете).

5. Начать управление сервером с помощью ssh (ввести команду в своем терминале):

```bash
ssh имя_пользователя@ip_сервера
```

После этой команды терминал запросит у вас пароль от пользователя (при вводе пароль виден не будет - это сделано специально в целях безопасности).

В качестве результата прикрепите скриншот терминала, когда вы подключились к серверу.

## Задание 2\* (необязательное)

Настройте свой ssh-клиент таким образом, чтобы можно было подключаться к серверу только такой командой (без ввода пароля):

```bash
ssh ваш_псевдоним_сервера
```

Подсказки:

1. Вам нужно узнать про `config` для ssh
2. Разобраться с командой `ssh-copy-id`
