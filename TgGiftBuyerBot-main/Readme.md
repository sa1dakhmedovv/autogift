❗ IMPORTANT
Due to recent changes, Telegram has started disabling the gift purchase functionality in bots when new gifts are released.
As a result, the autobuy feature may no longer work correctly.
Alternative: Use a userbot implementation with Telethon.
⚠️ This implementation is not provided in this repository.

To use the /refund command:

    Open the database (in the root of the repository).

    Go to the users table and change your status from user to admin.

    Go to the transactions table and copy the telegram_payment_charge_id of the transaction you want to refund.

    Return to the bot and run the command:

    /refund <telegram_payment_charge_id>

⚠️ Warning: If the bot's balance has fewer stars than the transaction amount, the refund will fail.

Alternative: Use the Telegram withdrawal bot. You must have at least 1000 stars available to withdraw.

❗ ВАЖНО
В связи с последними изменениями Telegram начал отключать возможность покупки подарков у ботов при выходе новых подарков.
Из-за этого функция autobuy может работать некорректно.
Альтернатива: использовать userbot на базе Telethon.
⚠️ Эта реализация не включена в данный репозиторий.

Чтобы воспользоваться командой /refund:

    Откройте базу данных (в корне репозитория).

    В таблице users измените status вашего аккаунта с user на admin.

    Перейдите в таблицу transactions и скопируйте telegram_payment_charge_id нужной транзакции.

    Вернитесь в бота и выполните команду:

    /refund <telegram_payment_charge_id>

⚠️ Важно: если на балансе бота меньше звёзд, чем в указанной транзакции — рефанд не выполнится.

Альтернатива: вывод средств через Telegram-бота. Требуется не менее 1000 звёзд на балансе для вывода.


> ⚠️ **Disclaimer (EN):**  
> This bot can potentially be used for fraudulent or unethical purposes.  
> I do **not host**, **administer**, or **control** this bot.  
> I bear **no responsibility** for any actions taken with this code.  
> The source code is **open-source** and provided **as is**, with **no guarantees or warranties**.  
> 🚫 **Telegram gifts for channels are not supported.** You can only send gifts to individual users (via `user_id`).

> ⚠️ **Предупреждение (RU):**  
> Этот бот может быть использован в мошеннических или недобросовестных целях.  
> Я **не размещаю**, **не администрирую** и **не контролирую** работу бота.  
> Я **не несу ответственности** за действия, связанные с этим кодом.  
> Исходный код распространяется **в открытом доступе** и предоставляется **"как есть"**, **без каких-либо гарантий**.  
> 🚫 **Подарки для Telegram-каналов не поддерживаются.** Вы можете отправлять подарки только отдельным пользователям (по `user_id`).

# 🎁 Gift Auto Buyer Bot

## 🔥 Description
**Gift Auto Buyer Bot** is a bot that automatically purchases gifts as soon as they become available, using the following settings:
- **Price Limit** — maximum price restriction.
- **Supply Limit** — available gift quantity restriction.
- **Number of Cycles** — number of purchase attempts.

Additionally, the bot supports **bulk gift purchases** with options to:
- Select which gift to buy.
- Specify the recipient (`user_id` in Telegram).
- Define the number of gifts to purchase.

## 🚀 Features
✅ Automatic monitoring and purchase of gifts based on defined parameters.
✅ Flexible settings for price, quantity, and cycle limits.
✅ Bulk purchase with recipient selection.
✅ Telegram ID support for targeted sending.
✅ Easy process management via a user-friendly interface.

## 📦 Installation
### 🔹 Requirements
- Python **3.12.8**
- pip (installed with Python)

### 🔹 Install dependencies
```sh
pip install -r requirements.txt
```

## 🛠 Configuration
Before running the bot, configure the settings in `config.py`:
```python
def load_config():
    return {
        "bot_token": '',
        "DATABASE_URL": 'sqlite:///user_data.db'
    }
```
- `bot_token` — your bot's Telegram API token.
- `DATABASE_URL` — database connection string (SQLite by default).

## ▶ Run
```sh
python main.py
```

## 📜 License
This project is distributed under the **MIT** license.

---
👤 **Author:** [neverwasbored](https://github.com/neverwasbored)

---

# 🎁 Бот для автоматической покупки подарков

## 🔥 Описание
**Gift Auto Buyer Bot** — это бот, который автоматически скупает подарки в момент их появления, используя заданные параметры:
- **Price Limit** — ограничение по цене.
- **Supply Limit** — ограничение по количеству доступных подарков.
- **Number of Cycles** — количество циклов для попыток покупки.

Кроме того, бот поддерживает **массовую покупку** подарков с возможностью указания:
- Какой подарок купить.
- Кому отправить (по `user_id` в Telegram).
- Количество подарков.

## 🚀 Возможности
✅ Автоматический мониторинг и покупка подарков по заданным параметрам.
✅ Гибкая настройка лимитов цены, количества и циклов.
✅ Массовая покупка с выбором получателей.
✅ Поддержка Telegram ID для адресной отправки.
✅ Запуск и контроль процессов через удобный интерфейс.

## 📦 Установка
### 🔹 Требования
- Python **3.12.8**
- pip (установлен вместе с Python)

### 🔹 Установка зависимостей
```sh
pip install -r requirements.txt
```

## 🛠 Конфигурация
Перед запуском настройте параметры в `config.py`:
```python
def load_config():
    return {
        "bot_token": '',
        "DATABASE_URL": 'sqlite:///user_data.db'
    }
```
- `bot_token` — API-токен вашего бота в Telegram.
- `DATABASE_URL` — строка подключения к базе данных (по умолчанию SQLite).

## ▶ Запуск
```sh
python main.py
```

## 📜 Лицензия
Этот проект распространяется под лицензией **MIT**.

---
👤 **Автор:** [neverwasbored](https://github.com/neverwasbored)

