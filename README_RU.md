<p align="center">
  <img src="https://img.shields.io/github/v/release/eviltrapgod/rigminator?include_prereleases&style=flat-square" alt="release">
  <img src="https://img.shields.io/github/last-commit/eviltrapgod/rigminator?style=flat-square" alt="last commit">
  <img src="https://img.shields.io/github/languages/top/eviltrapgod/rigminator?style=flat-square" alt="language">
  <img src="https://img.shields.io/github/license/eviltrapgod/rigminator?style=flat-square" alt="license">
</p>

<p align="center">
  <strong>Русский</strong> | <a href="README.md">English</a>
</p>

# **Проект закрыт за неимением команды**

---
---
---

# **Rigminator — Лёгкая и надёжная прошивка твоего Android-устройства**

---

**Rigminator** — это программа для быстрой и удобной прошивки Android-устройств. 
Простой интерфейс и расширяемая архитектура делают её идеальной как для новичков, так и для опытных пользователей.

## Как и на чем работает

* Использует `MTKclient` для работы с устройствами на базе MediaTek
* Интегрирует `ADB toolkit` для взаимодействия с Android-устройствами
* Поддерживает подключение и управление через USB
* Реализована на **`Python 3.13.5`** с использованием `PyQt6` для GUI
* Планируется расширение функционала с добавлением собственных обходов и модулей

## Как установить

### **Для работы требуется [Python 3.13.5](https://www.python.org/downloads/release/python-3135/)**

### Клонирование репозитория

```bash
git clone https://github.com/eviltrapgod/rigminator.git
cd rigminator
```

Или [Скачать]() архив

### Установка зависимостей

```bash
pip install -r requirements.txt
```

## Запуск
### **Windows**

```bash
python main.py
```

### **Linux / BSD**

```bash
python3 ./main.py
```

### **macOS (Darwin)**

```bash
python3 main.py
```

## Баг репорт

Если вы нашли ошибку или у вас есть предложения по улучшению, пожалуйста, сообщите нам через Telegram:
[@Rigminator\_bug\_bot](https://t.me/)

## Благодарности

**Проект создаётся и поддерживается командой Rigminator:**

* **@FAANGowner** — разработчик
* **@backupimei** — разработчик
* **@ellerstell4r** — разработчик
* **@Loadstring4ever** — разработчик

---

**Особая благодарность:**
* Увы..

## Лицензия

Этот проект распространяется под лицензией MIT.
Подробнее можно прочитать в файле [LICENSE](LICENSE).

## Поддержать проект

Если тебе нравится Regminator и ты хочешь поддержать разработку — это можно сделать:

* По реквизитам (добавь позже)
* Или просто передай доброе слово 😊


## 📌 TODO до первого релиза

### 🧱 Базовый GUI (PyQt6)
- [ ] Создать стартовое окно приложения с логотипом и кнопкой запуска
- [ ] Реализовать главное окно с вкладками ADB / Fastboot / Настройки
- [ ] Встроить лог-виджет для отображения статуса операций
- [ ] Форма выбора устройства / USB-порта (если применимо)

### 📦 Функции ADB
- [ ] Определение подключённых устройств через `adb devices`
- [ ] Получение базовой информации об устройстве (модель, Android, серийный номер)
- [ ] Кнопка перезагрузки устройства в обычный / recovery / bootloader режимы
- [ ] GUI-форма для прошивки через `adb sideload` (с выбором ZIP-файла)
- [ ] Поддержка shell-команд с подтверждением через диалоговое окно
- [ ] Вывод ADB-логов в реальном времени в интерфейсе

### 🧰 Функции Fastboot
- [ ] Определение fastboot-девайса через `fastboot devices`
- [ ] Кнопка прошивки одного раздела (`fastboot flash <partition> <file>`)
- [ ] Поддержка временной загрузки (`fastboot boot`)
- [ ] Возможность очистки раздела (`fastboot erase`)
- [ ] Кнопка перезапуска (`fastboot reboot`)
- [ ] Уведомления о результате операций (успех / ошибка)

### 🧠 Служебные функции и проверка окружения
- [ ] Автообновление списка устройств при подключении/отключении
- [ ] Проверка наличия и доступности утилит `adb`, `fastboot`, `mtkclient`
- [ ] Сохранение логов операций в файл `logs/session_<timestamp>.log`

### 🔒 Расширения безопасности и стабильности
- [ ] Блокировка выполнения критичных команд без подтверждения
- [ ] Отображение предупреждений при запуске опасных операций (wipe, erase и т.д.)
- [ ] Минимальная проверка валидности выбранных прошивочных файлов

