# 🤖 @RiyaksiyaRobot — O'rnatish Qo'llanmasi

## 📋 Talablar
- Python 3.10+
- python-telegram-bot 21.3+

---

## 🚀 O'rnatish

### 1. Kerakli paketlarni o'rnatish
```bash
pip install -r requirements.txt
```

### 2. `bot.py` faylini sozlash

Faylning yuqorisidagi `CONFIG` bo'limini to'ldiring:

```python
BOT_TOKEN = "YOUR_MAIN_BOT_TOKEN"   # BotFather dan olingan token
ADMIN_IDS  = [123456789]            # Sizning Telegram ID-ngiz
```

> Telegram ID olish: @userinfobot ga /start yuboring

### 3. Botni ishga tushirish
```bash
python bot.py
```

---

## ⚙️ Sozlamalar (Admin Panel)

`/panel` buyrug'ini yuboring va admin panelga kiring.

### 🤖 Reaksiya botlarini qo'shish (max 50 ta)
1. **Admin panel → ➕ Bot qo'shish** bosing
2. BotFather dan yangi bot yaratib, tokenini yuboring
3. Har bir bot **kanalga admin** bo'lishi SHART EMAS — faqat reaksiya bosadi

### 📢 Majburiy obuna kanalini o'rnatish
1. **Admin panel → 📢 Majburiy kanal** bosing
2. Kanal @username yuboring

### 📹 Qo'llanma video yuklash
1. **Admin panel → 📹 Qo'llanma video** bosing
2. Video yuboring

### 🎁 Sovg'a narxlarini o'zgartirish
1. **Admin panel → 🎁 Sovg'alar** bosing
2. Kerakli sovg'ani tanlang
3. Yangi ma'lumot yuboring: `emoji|nom|narx`
   - Misol: `🧸|Ayiq|6000`

---

## 🔢 Reaksiya Tizimi

| Bot raqami | Reaksiya |
|-----------|----------|
| Bot #1    | 👍 |
| Bot #2    | ❤️ |
| Bot #3    | 🔥 |
| Bot #4    | 😮 |
| Bot #5    | 😂 |
| Bot #6    | 🎉 |
| Bot #7    | 🤩 |
| Bot #8    | 😍 |
| Bot #9    | 👏 |
| Bot #10   | 💯 |
| Bot #11   | 🙏 |
| Bot #12   | 🚀 |
| Bot #13   | 👍 (Bot #1 ni takrorlaydi) |
| Bot #14   | ❤️ (Bot #2 ni takrorlaydi) |
| ...       | ... |

**Qoida:** 1-12 botlar bir-birining reaksiyasini qaytarmaydi.
13-chi bot esa 1-chi botning reaksiyasini bosadi va davom etadi.

---

## 📂 Fayl tuzilmasi

```
riyaksiya_bot/
├── bot.py          # Asosiy bot kodi
├── data.json       # Ma'lumotlar (avtomatik yaratiladi)
├── requirements.txt
└── README.md
```

---

## 👤 Foydalanuvchi uchun funksiyalar

| Tugma | Vazifasi |
|-------|---------|
| 🎯 Reaksiyalar | Kanal qo'shish/o'chirish/ko'rish |
| ⚙️ Sozlamalar | Reaksiyalar menyusi |
| 🛍 Yangi xizmatlar | Telegram/Instagram havolalar |
| 📖 Bot qo'llanmasi | Admin yuklaydigan video |
| 🎁 Sovg'alar olish | Sovg'alar ro'yxati va narxlar |

### Kanal qo'shgandan so'ng:
- **⚡ Reaksiya bosish** — muayyan postga reaksiya berish
- **🟢 Avtoni yoqish** — yangi postlarga avtomatik reaksiya

---

## 🛡️ Xavfsizlik

- Har bir foydalanuvchi faqat **o'z kanallarini** boshqara oladi
- Admin panel faqat `ADMIN_IDS` dagi foydalanuvchilarga ko'rinadi
- Bot tokenlar qisman ko'rsatiladi (`admin_list_bots`)

---

## ❓ Muammo va yechimlar

**Bot kanal postlarini ko'rmayapti (avto reaksiya ishlamayapti):**
- Botni kanalga `/setprivacy` - `disabled` qilganingizni tekshiring
- Yoki botni kanalga admin qilib qo'shing

**`set_message_reaction` xatosi:**
- Kanal ta'sir (reaction) yoqilgan bo'lishi kerak
- Premium emoji ishlatilamayapti (standart emoji ishlating)

---

*Yaratuvchi: @RiyaksiyaRobot*
