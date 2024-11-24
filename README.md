***Команды***


**Команда**	  ***< значание >***   -      **Описание**
```
🔍 **Основные команды:**
help - Справка о командах.
time - Показать время в разных городах мира
info <user_id|username> - Информация о пользователе
weather <город> - Узнать погоду в указанном городе

Формат вывода погоды:
🌡 ПОГОДА НА СЕГОДНЯ (Город)Z
⛅️ Текущая погода
↖️ Ветер и влажность
🌤 Прогноз на сегодня
☀️ Прогноз на завтра
☁️ Прогноз на послезавтра

spamattack <количество> -  Спам стикерами (Вы можете их указать в STICKER_ID)
stopspam - Оставновитьь спам есть он уже начался

🎵 **Музыка:**
music <название> - Поиск музыки
download <номер> - Скачать песню по номеру из результатов поиска
clear_downloads - Удалить скаченные песни


Примичание!: для работы поиска музыки необходимо скачать:
📝 Установите FFmpeg:
                - MacOS: brew install ffmpeg
                - Ubuntu: sudo apt-get install ffmpeg     ❗️ Загрузка может быть очень долгой!
                - Windows: скачайте с ffmpeg.org

🤖 **AI команды:**
set_model <model_name> - Установка модели AI (g4f, gemini, chatgpt)
gpt <текст> - Генерация ответа от AI
clear_context - Очистить контекст пользователя

🎮 **Развлечения:**
meme - Получить случайный мем


⚙️ **Настройки:**
set_prefix <символ> - Установить новый префикс команд

💡 **Примеры использования:**
• weather Москва
• info @username
• music In The End Linkin Park
```

Вы можете обновить префикс команды бота, используя /set_prefix <new_prefix>. По умолчанию, ***/.***

***ИИ*** 🪄

Бот поддерживает:

[Gemini](https://gemini.google.com/?hl=ru) (ИИ от Google) : Хороший

[G4F](https://github.com/techwithanirudh/g4f) (model = gpt-4-turbo ) : Не требует API

[ChatGPT](https://chatgpt.com/) (model = gpt-4-o ) : Надежный

 

Установите модель с помощью  ``/set_model <model_name>.``
    
Перед запуском напишите ``pip install -r requirements txt``

Еще одна команда которую вы можете добавить для спама в ЛС и в Чаты стикерами

*❗️* ***ВЫ МОЖЕТЕ ПОЛУЧИТЬ БАН ЗА СПАМ В ТЕЛЕГРАММЕ*** *❗️* 




*❗️* ***ВЫ МОЖЕТЕ ПОЛУЧИТЬ ТАКУЮ ОШИБКУ ВО ВРЕМЯ ИСПОЛЬЗОВАНИЯ API GEMINI ИЗ-ЗА КАТЕГОРИИ ВОПРОСА СЕКСУАЛЬНОГО и/или НЕЗАКОННОГО ХАРАКТЕРА*** *❗️* 

```
Oшибка при использовании Gemini: ("Invalid operation: The response.text quick accessor requires the response to contain a valid Part, but none were returned. The candidate's [finish_reason](https://ai.google.dev/api/generate-content#finishreason) is 3. The candidate's safety_ratings are: [category: HARM_CATEGORY_SEXUALLY_EXPLICIT\nprobability: HIGH\n, category: HARM_CATEGORY_HATE_SPEECH\nprobability: NEGLIGIBLE\n, category: HARM_CATEGORY_HARASSMENT\nprobability: NEGLIGIBLE\n, category: HARM_CATEGORY_DANGEROUS_CONTENT\nprobability: NEGLIGIBLE\n].", [category: HARM_CATEGORY_SEXUALLY_EXPLICIT
probability: HIGH
, category: HARM_CATEGORY_HATE_SPEECH
probability: NEGLIGIBLE
, category: HARM_CATEGORY_HARASSMENT
probability: NEGLIGIBLE
, category: HARM_CATEGORY_DANGEROUS_CONTENT
probability: NEGLIGIBLE
])
```
Ошибка, которую вы получили, связана с системой безопасности API Gemini (Google Generative AI). Она блокирует ответы, если они содержат или могут быть интерпретированы как опасные или запрещенные темы. В данном случае проблема связана с категорией "сексуально-эксплицитный контент" (HARM_CATEGORY_SEXUALLY_EXPLICIT) с высокой вероятностью.*




Бот при первом запуске попросит ваш номер телефона для входа в аккаунт и введите код потверждения для! Если вы зашли в аккаунт и хотете поменять аккаунт, то удалите файлы mybot.session (все файлы с этим названием) 

***[Поддержать автора](https://www.donationalerts.com/r/adolmi)***
