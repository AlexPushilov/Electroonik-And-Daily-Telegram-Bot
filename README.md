# Electroonik-And-Daily-Telegram-Bot
Don't copy this code pls


На текущее время бот работает не штатно!

Имя бота в телеграме: TimetableDiary344
Имя как пользователя(с идентификатором через@): @diary_344_bot

Функционал: По текущему времени бот выводит урок, проходящий сейчас, следующий урок и дату. При выборе другой кнопки выводит расписание на день.

Принцип работы: 1) При выводе команды /start бот берёт Telegram ID пользователя и складывает его в переменную us_id. После этого из базы данных изымаются все ID зарегистрированных в системе бота пользователи.
2) При при отсутствии ID в бд, пользователь отсылается на регистрацию в 3 этапа.
На каждом этапе регистрации, при вводе неправильных значений происходит рекурсивный функции запроса значения и проверка.
3) Клавиатура согласия взаимодействия удаляется после нажатия кнопки.
4) Когда пользователь заканчивает регистрауию или числится по ID в бд, он получает доступ к клавиатуре кнопок (не в сообщениях)
5) Через модуль datetime и имопрт данных из базы данных пользователю выводятся соответствующие значения
6) Прсле этого бот циклически работает на вывод уроков и расписания
