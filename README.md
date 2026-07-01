#english translatios are furture down


# Sentinel 2

> یک برنامه سبک برای مانیتورینگ شبکه که به شما کمک می‌کند دستگاه‌های متصل به شبکه محلی خود را شناسایی کنید، فعالیت آن‌ها را به صورت زنده مشاهده کنید، سازنده آن‌ها را تشخیص دهید و اطلاعات آن‌ها را در یک پایگاه داده ذخیره کنید.

---

## معرفی

Sentinel 2 یک پروژه متن‌باز نوشته شده با Python است که با هدف یادگیری شبکه، امنیت سایبری و تحلیل بسته‌های شبکه توسعه داده شده است.

این برنامه به صورت مداوم شبکه را اسکن می‌کند، دستگاه‌های متصل را شناسایی می‌کند، ترافیک شبکه را بررسی کرده و اطلاعات آن‌ها را در یک رابط گرافیکی نمایش می‌دهد.

---

## قابلیت‌ها

- اسکن خودکار شبکه
- Packet Sniffing
- تشخیص آنلاین یا آفلاین بودن دستگاه‌ها
- ذخیره اطلاعات دستگاه‌ها
- تشخیص شرکت سازنده دستگاه‌ها (Vendor)
- شمارش بسته‌های شبکه
- آمار پروتکل‌ها
- اعلان‌های ویندوز
- نمایش جزئیات دستگاه‌ها
- تاریخچه بسته‌ها
- رابط گرافیکی PySide6
- ساختار ماژولار

---

## تفاوت Sentinel 1 و Sentinel 2

### Sentinel 1

یک الگوریتم بسیار ساده برای مانیتورینگ شبکه که می‌توانست:

- شبکه را اسکن کند.
- دستگاه‌های متصل را پیدا کند.
- آن‌ها را با لیست سفید (Whitelist) مقایسه کند.

هدف اصلی آن یادگیری مفاهیم اولیه شبکه بود.

---

### Sentinel 2

Sentinel 2 نسخه‌ای کاملاً بازطراحی شده است.

در این نسخه پروژه از یک اسکنر ساده به یک نرم‌افزار کامل تبدیل شده است که شامل:

- Packet Sniffing
- رابط گرافیکی
- پایگاه داده
- تاریخچه دستگاه‌ها
- تشخیص Vendor
- اعلان‌ها
- آمار پروتکل‌ها
- ساختار حرفه‌ای‌تر
- قابلیت توسعه آسان‌تر

---

## نصب

دریافت پروژه

```bash
git clone https://github.com/yourusername/Sentinel_2.git

cd Sentinel_2
```

ساخت محیط مجازی

### ویندوز

```powershell
python -m venv .venv

.venv\Scripts\activate
```

### لینوکس

```bash
python3 -m venv .venv

source .venv/bin/activate
```

نصب کتابخانه‌ها

### ویندوز

```powershell
pip install -r requirements.txt
```

### لینوکس

```bash
pip3 install -r requirements.txt
```

اجرای برنامه

### ویندوز

```powershell
python main.py
```

### لینوکس

```bash
python3 main.py
```

---

## کتابخانه‌های مورد نیاز

- PySide6
- Scapy
- psutil
- win11toast (فقط ویندوز)

---

## Sentinel 3

نسخه سوم ادامه Sentinel 2 خواهد بود و از ابتدا نوشته نمی‌شود.

برخی قابلیت‌های برنامه‌ریزی شده:

- Deep Packet Inspection (DPI)
- تشخیص وب‌سایت‌های بازدید شده
- نمودارهای زنده مصرف پهنای باند
- Timeline بسته‌ها
- رابط کاربری مدرن‌تر
- بانک اطلاعاتی پیشرفته‌تر
- جستجوی بسته‌ها
- تاریخچه فعالیت
- آمار کامل‌تر
- انیمیشن‌های رابط کاربری

---

## هدف پروژه

این پروژه با هدف یادگیری و تقویت مهارت‌ها در زمینه‌های زیر ساخته شده است:

- شبکه‌های کامپیوتری
- امنیت سایبری
- تحلیل Packet
- Python
- طراحی نرم‌افزارهای دسکتاپ
- برنامه‌نویسی چندنخی (Multithreading)

---

## License

MIT License






ENGLISH VERSION


# Sentinel 2

> A lightweight network monitoring application that helps you discover devices on your local network, monitor their activity in real time, identify vendors, and maintain a persistent device database.

---

## Overview

Sentinel 2 is a Python-based network monitoring tool built for learning, experimentation, and cybersecurity practice.

It continuously scans your local network, detects connected devices, captures network traffic, and displays useful information through a desktop GUI.

The project was built from scratch as a way to learn networking, multithreading, packet analysis, GUI development, and Python application design.

---

## Features

- Automatic network discovery (ARP Scanner)
- Live packet sniffing
- Online / Offline device detection
- Device database (JSON)
- Vendor identification using OUI database
- Packet counters
- Protocol statistics (TCP, UDP, ICMP...)
- Windows notifications
- Device details
- Packet history
- Modular architecture
- Desktop GUI (PySide6)

---

## Sentinel 1 vs Sentinel 2

### Sentinel 1

A very simple network monitoring algorithm that could:

- Scan a local network
- Detect connected devices
- Compare discovered devices against a whitelist

Its purpose was simply learning the basics of networking.

---

### Sentinel 2

Sentinel 2 is a complete redesign.

Instead of being a simple scanner, it became a modular desktop application featuring:

- Live packet sniffing
- GUI
- Persistent database
- Device history
- Vendor lookup
- Notifications
- Protocol statistics
- Better architecture
- Easier future expansion

---

## Installation

Clone the repository

```bash
git clone https://github.com/yourusername/Sentinel_2.git

cd Sentinel_2
```

Create a virtual environment (recommended)

### Windows

```powershell
python -m venv .venv

.venv\Scripts\activate
```

### Linux

```bash
python3 -m venv .venv

source .venv/bin/activate
```

Install dependencies

### Windows

```powershell
pip install -r requirements.txt
```

### Linux

```bash
pip3 install -r requirements.txt
```

Run

### Windows

```powershell
python main.py
```

### Linux

```bash
python3 main.py
```

---

## Required Packages

- PySide6
- scapy
- psutil
- win11toast (Windows only)

Install manually:

### Windows

```powershell
pip install PySide6 scapy psutil win11toast
```

### Linux

```bash
pip3 install PySide6 scapy psutil
```

---

## Project Structure

```
Sentinel_2
│
├── main.py
├── gui.py
├── scanner.py
├── sniffer.py
├── devices.py
├── database.py
├── notifications.py
├── vendor.py
├── database/
└── vendors.json
```

---

## Sentinel 3 (Planned)

Sentinel 3 will build upon Sentinel 2 instead of replacing it.

Planned features include:

- Deep Packet Inspection (DPI)
- Website detection
- Live bandwidth graphs
- Packet timeline
- Improved Windows 11 interface
- Device aliases & notes
- Better database
- Packet search
- Activity history
- Better statistics
- Animated interface
- More advanced network analysis

---

## Purpose

This project was created primarily to improve my understanding of:

- Computer Networking
- Cybersecurity
- Packet Analysis
- Python
- Desktop Application Development
- Multithreading
- GUI Design

---

## License

MIT License
