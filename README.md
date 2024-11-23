***Команды***


**Команда**	  ***< значание >***   -      **Описание**
```
/help	- Справка.
/info	- Информация о пользователе который ввел команду;
/time	- Показывает текущее время в МСК;
/weather < город > - Узнать погоду в <город>;
/set_prefix < символ > - Изменить префикс на < символ > (По умолчанию " / ");
/set_model < model > - Устанавливает модель ИИ (gemini, g4f, meta);
/gpt < text > - Спросить у ИИ (< model >) вопрос;
/clear_context - Очистить контекст пользователя.

Вместо </> будет префикс который вы установили!
```

Вы можете обновить префикс команды бота, используя /set_prefix <new_prefix>. По умолчанию, ***/.***

***ИИ*** 🪄

Бот поддерживает:

[Gemini](https://gemini.google.com/?hl=ru) (ИИ от Google) : Хороший

[G4F](https://github.com/techwithanirudh/g4f) (model = gpt-3.5-turbo ) : Не требует API

[ChatGPT](https://chatgpt.com/) (model = gpt-3.5-turbo ) : Надежный

 

Установите модель с помощью  ```/set_model <model_name>.```
    
Перед запуском напишите ```pip install -r requirements txt```

Еще одна команда которут вы можете добавить для спама в ЛС и в Чаты стикерами

*❗️* ***ВЫ МОЖЕТЕ ПОЛУЧИТЬ БАН ЗА СПАМ В ТЕЛЕГРАММЕ*** *❗️* 


```

# Список авторизованных пользователей
allowed_user_ids = [2161024343, 2244396277]  # Замените на ID пользователей, которым разрешено использовать команды

# Флаг для остановки спама
stop_spam_flag = False

@app.on_message(filters.command("spamattack"))
async def spamattack(client, message):
    global stop_spam_flag

    # Проверяем, есть ли отправитель в списке разрешённых пользователей
    if message.from_user.id not in allowed_user_ids:
        await message.reply("❗ У вас нет прав для использования этой команды.")
        return

    # Разделяем команду и аргумент
    args = message.text.split(maxsplit=1)

    # Если аргумент не указан
    if len(args) < 2:
        await message.reply("❗ Укажите количество сообщений, например: /spamattack 5")
        return

    try:
        # Пробуем преобразовать аргумент в число
        count = int(args[1].strip())

        if count <= 0:
            await message.reply("❗ Количество сообщений должно быть больше нуля.")
            return

        # Сбрасываем флаг перед началом спама
        stop_spam_flag = False

        await message.reply(f"Начинаю спамить {count} сообщений!")

        # Цикл отправки сообщений
        for i in range(count):
            if stop_spam_flag:
                await message.reply("⚠️ Спам остановлен.")
                return

            await client.send_sticker(message.chat.id, STICKER_ID)  # Укажите ваш ID стикера
            await asyncio.sleep(1)  # Пауза между сообщениями

        await message.reply("✅ Спам завершён!")
    except ValueError:
        await message.reply("❗ Укажите корректное число, например: /spamattack 5")

@app.on_message(filters.command("stopspam"))
async def stopspam(client, message):
    global stop_spam_flag

    # Проверяем, есть ли отправитель в списке разрешённых пользователей
    if message.from_user.id not in allowed_user_ids:
        await message.reply("❗ У вас нет прав для использования этой команды.")
        return

    # Устанавливаем флаг для остановки
    stop_spam_flag = True
    await message.reply("⛔ Спам будет остановлен.")


```


Бот при первом запуске попросит BOT TOKEN или же ваш номер телефона для входа в аккаунт и введите код потверждения для! Если вы зашли в аккаунт и хотете поменять аккаунт, то удалите файлы mybot.session (все файлы с этим названием) 

***[Поддержать автора](https://www.donationalerts.com/r/adolmi)***
