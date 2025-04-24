# 🛰 Практична робота 5 — gRPC-сервіс повідомлень (C# / .NET 8)

Цей проєкт — реалізація практичної роботи №5: **gRPC-служба обміну текстовими повідомленнями** на мові C# (.NET 8) згідно з методичкою.

## 📦 Склад проєкту

- `GrpcMessageServer` — gRPC-сервер, що приймає потік повідомлень і повертає `echo` + лічильник
- `GrpcMessageClient` — консольний клієнт, який надсилає повідомлення у стрімі

---

## 🛠 Технології

- .NET 8
- C#
- gRPC (client & server streaming)
- Protocol Buffers (`.proto`)
- Visual Studio 2022+

---

## 🚀 Як запустити проєкт

### 📌 Перед запуском

> Переконайся, що в тебе:
> - Установлено .NET 8 SDK
> - Встановлено Visual Studio з workload "ASP.NET and web development"

---

### ▶ Запуск сервера

1. Встанови `GrpcMessageServer` як **Startup Project**
2. У файлі `launchSettings.json` встанови:
   ```json
   "applicationUrl": "http://localhost:5000"
