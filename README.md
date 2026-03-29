# 👻 Ghostgram — Unofficial Telegram iOS Client

![License](https://img.shields.io/github/license/Ogshty/ghostgram?style=flat-square)
![Swift](https://img.shields.io/badge/Swift-5.10-orange?style=flat-square)
![Platform](https://img.shields.io/badge/Platform-iOS%2015.0+-blue?style=flat-square)
![Build](https://img.shields.io/github/actions/workflow/status/Ogshty/ghostgram/build.yml?branch=main&style=flat-square)

**Ghostgram** — это модифицированный клиент Telegram для iOS, ориентированный на стабильность и автоматизированную сборку. Проект базируется на официальном исходном коде Telegram и адаптирован для удобной компиляции через GitHub Actions.

---

## ✨ Особенности
* **Автоматизация:** Полностью настроенный CI/CD пайплайн (GitHub Actions) для сборки `.ipa`.
* **Xcode 16 Ready:** Поддержка актуальных инструментов разработки 2026 года.
* **Unsigned Build:** Возможность сборки без платного аккаунта разработчика Apple (использование фейковых сертификатов).
* **Apple Silicon Optimized:** Оптимизировано для сборки на раннерах M1/M2/M3.

---

## 🛠 Требования для локальной сборки
Если вы решите собирать проект на своем Mac, вам понадобятся:
* **macOS 15.0+**
* **Xcode 16.0+**
* **Python 3.10+**
* **Bazel** (рекомендуется устанавливать через `bazelisk`)

---

## 🚀 Быстрый старт (GitHub Actions)
Самый простой способ получить готовый `.ipa` — использовать встроенный Workflow:

1.  Сделайте **Fork** этого репозитория.
2.  Перейдите во вкладку **Actions**.
3.  Выберите ворклоу `CI - Build Telegram iOS (Unsigned)`.
4.  Нажмите **Run workflow**. 
5.  По завершении скачайте артефакт `Telegram-iOS-Unsigned` в нижней части страницы запуска.

---

## 💻 Локальная компиляция

### 1. Клонирование репозитория
```bash
git clone --recursive [https://github.com/Ogshty/ghostgram.git](https://github.com/Ogshty/ghostgram.git)
cd ghostgram
