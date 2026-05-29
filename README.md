🇷🇺 [Русский](#proxy-tester) | 🇬🇧 [English](#proxy-tester-1)

---

# 🛡️ Proxy Tester

**Многопоточный тестер прокси-конфигов с поддержкой VLESS, VMESS, Trojan и Shadowsocks.**

Быстрый инструмент для массовой проверки работоспособности и геолокации прокси-серверов. Читает ссылки из файла `servers.txt`, проверяет доступность через TCP-пинг, поднимает Xray-core и тестирует реальное соединение. Итоговый результат сохраняется в удобном интерактивном HTML-отчёте.

![Platform](https://img.shields.io/badge/Platform-Windows-lightgrey) ![Python](https://img.shields.io/badge/Python-3.7+-blue.svg) ![License](https://img.shields.io/badge/License-MIT-green)

---

## ✨ Возможности

- 🚀 **Высокая производительность** – эффективно тестирует 30–50 серверов одновременно.
- 🔍 **Предварительный TCP-пинг** – асинхронная проверка доступности сервера перед тестом.
- 🌍 **Геолокация** – определение страны, города, провайдера и IP для каждого работающего прокси.
- 📊 **Интерактивный HTML-отчёт** – сортировка по столбцам, фильтрация по странам и статусу, поиск.
- 🔗 **Копирование ссылок** – быстрый экспорт рабочих URL прямо из отчёта.
- 🧩 **Поддержка протоколов**:
  - **VLESS** (tcp/ws/grpc/h2 + tls/reality)
  - **VMESS** (tcp/ws/grpc/h2 + tls)
  - **Trojan** (tcp/ws/grpc + tls)
  - **Shadowsocks** (все методы шифрования)
- 🧹 **Автоматическая очистка** – временные конфиги Xray удаляются после теста.

---

## 📝 Последовательность запуска 

#### 1) ⚙️ Установка зависимостей
```powershell
.\requirements.ps1
```

#### 2) 📋 Добавление серверов
Отредактируйте файл `servers.txt` и вставьте свои прокси (каждая с новой строки).

#### 3) 🚀 Запуск тестирования
```powershell
python proxy-tester.py
```

---

## 📊 Результаты

После завершения теста создаётся HTML-отчёт вида `report_20260101_120000.html` со следующими возможностями:

- 📈 **Сводная статистика** (всего / рабочих / нерабочих / стран).
- 🌍 **Фильтрация по странам** (кнопки с флагами).
- ✅❌ **Фильтр по статусу** (рабочие / нерабочие).
- 🔍 **Поиск** по имени, IP, провайдеру.
- 📊 **Сортировка** по любому столбцу (клик по заголовку).
- 📋 **Копирование ссылки** в один клик.

![PREVIEW](https://raw.githubusercontent.com/tglagcs/Proxy-Tester/refs/heads/main/PREVIEW.png)

---

## 🤝 Вклад в проект

Pull request'ы приветствуются! Если вы нашли баг или хотите предложить улучшение, создайте [Issue](https://github.com/tglagcs/Proxy-Tester/issues).

---
---

# 🛡️ Proxy Tester

**Multi-threaded proxy config tester with support for VLESS, VMESS, Trojan, and Shadowsocks.**

A fast tool for bulk checking proxy server availability and geolocation. It reads links from `servers.txt`, verifies connectivity via TCP ping, launches Xray-core, and tests the real connection. Results are saved in a convenient interactive HTML report.

![Platform](https://img.shields.io/badge/Platform-Windows-lightgrey) ![Python](https://img.shields.io/badge/Python-3.7+-blue.svg) ![License](https://img.shields.io/badge/License-MIT-green)

---

## ✨ Features

- 🚀 **High performance** – efficiently tests 30–50 servers simultaneously.
- 🔍 **TCP pre-ping** – asynchronously checks server availability before the full test.
- 🌍 **Geolocation** – detects country, city, ISP, and IP for each working proxy.
- 📊 **Interactive HTML report** – sortable columns, country and status filters, search.
- 🔗 **Link copying** – quickly export working URLs directly from the report.
- 🧩 **Protocol support**:
  - **VLESS** (tcp/ws/grpc/h2 + tls/reality)
  - **VMESS** (tcp/ws/grpc/h2 + tls)
  - **Trojan** (tcp/ws/grpc + tls)
  - **Shadowsocks** (all cipher methods)
- 🧹 **Auto cleanup** – temporary Xray configs are deleted after the test.

---

## 📝 How to Run

#### 1) ⚙️ Install dependencies
```powershell
.\requirements.ps1
```

#### 2) 📋 Add servers
Edit the `servers.txt` file and paste your proxies (one per line).

#### 3) 🚀 Start testing
```powershell
python proxy-tester.py
```

---

## 📊 Results

After the test completes, an HTML report named `report_20260101_120000.html` is created with the following features:

- 📈 **Summary statistics** (total / working / failed / countries).
- 🌍 **Country filter** (flag buttons).
- ✅❌ **Status filter** (working / failed).
- 🔍 **Search** by name, IP, or ISP.
- 📊 **Sorting** by any column (click the header).
- 📋 **One-click link copy**.

![PREVIEW](https://raw.githubusercontent.com/tglagcs/Proxy-Tester/refs/heads/main/PREVIEW.png)

---

## 🤝 Contributing

Pull requests are welcome! If you found a bug or want to suggest an improvement, open an [Issue](https://github.com/tglagcs/Proxy-Tester/issues).
