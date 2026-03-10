<div align="center">

# 🛡️ Enterprise Incident Tracker
**Комплексное десктопное решение для управления корпоративной безопасностью**

[![Python](https://img.shields.io/badge/Python-3.10-blue.svg?style=for-the-badge&logo=python&logoColor=white)](#)
[![PyQt5](https://img.shields.io/badge/GUI-PyQt5-green.svg?style=for-the-badge&logo=qt&logoColor=white)](#)
[![SQLite](https://img.shields.io/badge/Database-SQLite3-003B57.svg?style=for-the-badge&logo=sqlite&logoColor=white)](#)
[![Security](https://img.shields.io/badge/Security-HWID_%7C_Bcrypt-red.svg?style=for-the-badge)](#)

*Автоматизация работы служб безопасности (СБ), ЧОП и управляющих компаний. Забудьте о потерянных бумажных рапортах и хаосе в Excel.*

[Связь с разработчиком (Telegram)](https://t.me/Yaroslav_GIT) • [Скачать Demo](https://github.com/YYaroslavSSolovev/Enterprise-Incident-Tracker/releases/tag/v1.0.0)

</div>

---

## 📸 Интерфейс системы

<div align="center">
  <h3>1. Рабочее пространство (Main & Dashboard)</h3>
  
  <!-- СКРИНШОТ 1: Главное Окно (Main Window) -->
  <img src="screenshots/main_window.png" alt="Главное Окно" width="800" style="border-radius: 8px; box-shadow: 0 4px 8px rgba(0,0,0,0.2); margin-bottom: 10px;">
  <p><i>Единое окно для управления всеми модулями (Emergency, Breach, Suspicious Activity)</i></p>

  <br>

  <!-- СКРИНШОТ 2: Окно Дашборда (Dashboard) -->
  <img src="screenshots/dashboard.png" alt="Аналитический дашборд" width="800" style="border-radius: 8px; box-shadow: 0 4px 8px rgba(0,0,0,0.2); margin-bottom: 10px;">
  <p><i>Интерактивный Dashboard: мониторинг активных инцидентов и просроченных задач в реальном времени</i></p>
</div>

<br><hr><br>

<div align="center">
  <h3>2. Безопасность и Вход (Security)</h3>
  <table style="border: none;">
    <tr>
      <td align="center" width="50%">
        <!-- СКРИНШОТ 3: Окно лицензии (HWID) -->
        <img src="screenshots/license_window.png" alt="Окно активации лицензии" width="100%" style="border-radius: 8px;">
        <br><i>Привязка к оборудованию (HWID Protection)</i>
      </td>
      <td align="center" width="50%">
        <!-- СКРИНШОТ 4: Окно аутентификации (Login) -->
        <img src="screenshots/login_window.png" alt="Окно авторизации" width="100%" style="border-radius: 8px;">
        <br><i>Защищенный вход (Bcrypt Auth)</i>
      </td>
    </tr>
  </table>
</div>

<br><hr><br>

<div align="center">
  <h3>3. Администрирование (Administration)</h3>
  <table style="border: none;">
    <tr>
      <td align="center" width="50%">
        <!-- СКРИНШОТ 5: Окно управления пользователями (Users) -->
        <img src="screenshots/users_window.png" alt="Управление пользователями" width="100%" style="border-radius: 8px;">
        <br><i>Role-Based Access Control (Управление ролями)</i>
      </td>
      <td align="center" width="50%">
        <!-- СКРИНШОТ 6: Окно аудита (Audit Log) -->
        <img src="screenshots/audit_window.png" alt="Журнал аудита" width="100%" style="border-radius: 8px;">
        <br><i>Audit Log (Контроль действий персонала)</i>
      </td>
    </tr>
  </table>
</div>

<br><hr><br>

<div align="center">
  <h3>4. Учёт инцидентов (Reporting)</h3>
  <!-- СКРИНШОТ 7: Форма репорта (Report Form) -->
  <img src="screenshots/report_window.png" alt="Форма создания отчета" width="800" style="border-radius: 8px; box-shadow: 0 4px 8px rgba(0,0,0,0.2); margin-bottom: 10px;">
  <p><i>Многовкладочная форма создания рапорта (фиксация ущерба, задач, потерь и вложений)</i></p>
</div>

---

## 💼 Почему бизнесу нужна эта система?

До 70% важной информации об инцидентах на объектах теряется из-за человеческого фактора или использования разрозненных мессенджеров. **Enterprise Incident Tracker** решает эту проблему:

* ⏱️ **Отчеты за 1 клик:** Автоматическая генерация профессиональных PDF-рапортов с QR-кодами для руководства.
* 🔒 **Абсолютная конфиденциальность:** Программа работает полностью **offline**. Данные не передаются в облако и хранятся в защищенной локальной базе (SQLite).
* 👁️ **Защита от саботажа:** Встроенный *Audit Log* фиксирует каждый клик. Сотрудник не сможет удалить инцидент или подменить данные незаметно.
* 🎯 **Контроль поручений:** Встроенный таск-трекер для отслеживания реакций на инциденты (кто должен устранить последствия и в какой срок).

---

## ✨ Ключевой функционал

### 1. Учет трех типов инцидентов
* **🚨 Emergency Incidents (ЧС)**: Фиксация аварий, ущерба и потерь.
* **🛡️ Security Breaches (Нарушения периметра)**: Учет попыток проникновения и действий нарушителей.
* **👁️‍🗨️ Suspicious Activity (Подозрительная активность)**: Работа на опережение и планирование усиления охраны.

### 2. Строгая ролевая модель (RBAC)
* **👑 Administrator**: Полный доступ. Управление пользователями, аудит, снятие блокировок.
* **🏢 Facility Manager**: Доступ только к отчетам своего объекта + аналитика.
* **👨‍💻 Operator**: Режим "read/write" только для своего объекта без доступа к настройкам.

### 3. Защита файлов и вложений
Возможность прикреплять к рапортам фотографии и документы. Система автоматически проверяет файлы на целостность алгоритмом `SHA-256`, исключая подмену доказательств.

---

## 🛠 Технологии под капотом (Для IT-специалистов)

* **UI Layer:** PyQt5 (строгий корпоративный интерфейс, нативная отрисовка).
* **Data Layer:** Чистый SQL (SQLite3) с использованием Prepared Statements (нулевой риск SQL-инъекций). Никаких тяжелых ORM.
* **Cryptography:** `bcrypt` (12 раундов) для паролей, `hashlib` для файлов, `secrets` для генерации.
* **Security:** Программная защита от Brute-Force атак (таймаут после 5 попыток).
* **Compiler:** Бинарная компиляция через `Nuitka` (C-level). Исходный код недоступен для реверс-инжиниринга.

---

## 📥 Скачать Демо-версию

Данный программный комплекс является **коммерческим продуктом**. Исходный код закрыт.

Вы можете бесплатно протестировать работу системы:
1. Перейдите в раздел [**Releases**](https://github.com/YYaroslavSSolovev/Enterprise-Incident-Tracker/releases) (справа).
2. Скачайте архив `Enterprise_Tracker_Win64.zip` и распакуйте его на ПК с Windows.
3. Запустите файл `.exe`.
4. Система выдаст вам уникальный идентификатор вашего оборудования (**HWID**).
5. Напишите мне в Telegram и отправьте HWID — я выдам вам **бесплатный тестовый ключ**.

---

## 🤝 Заказ разработки и покупка ПО

Я открыт для B2B сотрудничества и фриланс-заказов. 

Что я предлагаю:
* 🛒 **Покупка готовой системы** (выдача безлимитных лицензий на ваши ПК).
* ⚙️ **Кастомизация ПО** под бизнес-процессы вашей компании (добавление ваших логотипов, новых типов отчетов, интеграция с вашими серверами).
* 💻 **Покупка исходного кода** (Source Code) для вашей in-house команды разработки.
* 🛠️ **Разработка десктопного ПО с нуля** на Python (PyQt/PySide).

**Свяжитесь со мной для обсуждения проекта:**

💬 **Telegram:** [@Yaroslav_GIT](https://t.me/Yaroslav_GIT)  

<br>

<div align="center">
  <i>Enterprise Incident Tracker © 2026. All Rights Reserved.</i>
</div>
