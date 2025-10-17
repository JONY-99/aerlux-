# aerlux-
# 🌐 AERLUX — Dasturiy ta'minotda innovatsion yondashuv!

**AERLUX** — bu zamonaviy, ko‘p tilli (UZ/RU/EN) web sahifa bo‘lib, dasturiy yechimlar, Telegram botlar va web ilovalar yaratish bo‘yicha xizmatlarni taqdim etadi.  
Sayt yagona HTML fayl asosida ishlab chiqilgan va to‘liq responsiv (telefon, planshet va kompyuter ekranlariga mos).

---

## 🚀 Asosiy imkoniyatlar

✅ **To‘liq responsiv dizayn**  
Navbar, menyular, va til tanlash funksiyasi barcha ekranlarda moslashadi.

✅ **Ko‘p tilli interfeys (UZ / RU / EN)**  
Matnlar avtomatik tarzda tilga qarab yangilanadi (i18n tizimi orqali).

✅ **Yorug‘ / qorong‘i rejim (Light / Dark Mode)**  
Foydalanuvchi tanlagan tema `localStorage` orqali saqlanadi.

✅ **Telegram bilan integratsiya**  
Kontakt formasi yuborilganda ma’lumotlar to‘g‘ridan-to‘g‘ri Telegram guruh yoki kanalga yuboriladi.

✅ **Dinamik loyihalar bo‘limi**  
Loyihalar haqidagi ma’lumotlar JavaScript orqali avtomatik render qilinadi.

✅ **Yuqori UX va animatsiya**  
Intersection Observer orqali smooth “scroll reveal” effektlar mavjud.

---

## 🧱 Texnologik stek

| Qatlam | Tavsif |
|--------|---------|
| **Frontend** | HTML5, CSS3, Vanilla JavaScript |
| **Shriftlar** | Inter (Google Fonts) |
| **Stil** | CSS o‘zgaruvchilari, media query, gradient fon |
| **Animatsiya** | IntersectionObserver |
| **Ma’lumot yuborish** | Telegram Bot API |
| **Saqlash** | LocalStorage (til va tema uchun) |

---

## 📂 Loyihaning tuzilishi

aerlux/
├── index.html # Asosiy sahifa (bitta HTML fayl)
├── /assets # (ixtiyoriy) rasm va ikonlar
└── README.md # Hujjat (ushbu fayl)

yaml
Copy code

---

## ⚙️ Ishga tushirish

### 1️⃣ Lokal ko‘rish
Faylni brauzerda bevosita ochish mumkin.  
Yoki terminal orqali mini-server ishga tushirish:
```bash
python3 -m http.server 8000
# so‘ng http://localhost:8000 manzilini oching
💬 Telegram konfiguratsiyasi
Kontakt formasining ishlashi uchun:

@BotFather orqali yangi bot yarating

Bot tokenini oling

Yangi Telegram guruh yarating va botni unga qo‘shing

Guruhga bitta test xabar yuboring

Quyidagi manzilni brauzerda oching:

bash
Copy code
https://api.telegram.org/bot<YOUR_TOKEN>/getUpdates
chat.id qiymatini toping (odatda -100XXXXXXXXXX ko‘rinishida bo‘ladi)

index.html ichidagi quyidagi qismini o‘zgartiring:

js
Copy code
const TELEGRAM_BOT_TOKEN = "YOUR_BOT_TOKEN";
const TELEGRAM_CHAT_ID   = "-100XXXXXXXXXX";
🌍 Ko‘p tilli tizim (i18n)
Barcha matnlar quyidagi I18N obyekti ichida saqlanadi:

js
Copy code
const I18N = {
  uz: { "nav.home": "Bosh sahifa", ... },
  ru: { "nav.home": "Главная", ... },
  en: { "nav.home": "Home", ... }
};
Til o‘zgartirilganda:

js
Copy code
setLang("ru");
Matnlar avtomatik yangilanadi, tanlov esa localStorageda saqlanadi.

📱 Mobil menyu va tillar
Kompyuterda: menyu va tillar yonma-yon chiqadi

Telefon / planshetda:

menyu “burger” ko‘rinishida ochiladi

tillar esa dropdown oynada ko‘rsatiladi

Har bir elementda ARIA atributlar mavjud (masalan, aria-expanded, aria-controls) — bu accessibility uchun.

💌 Kontakt formasi
Forma ma’lumotlarini quyidagi tarzda yuboradi:

js
Copy code
fetch(`https://api.telegram.org/botTOKEN/sendMessage?chat_id=CHAT_ID&text=...`);
Agar CORS bloklasa, tizim no-cors yoki Image() orqali fallback yuborishni amalga oshiradi.

🧠 Moslashtirish (Customization)
Bo‘lim	Qanday o‘zgartirish mumkin
Loyihalar	<script> dagi PROJECTS massivini tahrirlang
Ranglar	:root dagi CSS o‘zgaruvchilarni o‘zgartiring
Logo / nom	<div class="brand"> ichidagi matn
Kontakt ma’lumotlar	#contact bo‘limidagi <a> teglarida
Formani o‘zgartirish	#contactForm strukturasini moslang

🧾 Loyiha haqida
Loyiha nomi: AERLUX — Dasturiy ta’minotda innovatsion yondashuv
Yo‘nalish: Web development / Telegram bot / SaaS platformalar
Muallif: Sardor Karimjonov
Sayt: https://aerlux.uz
Telegram: @AERLUXuz
Email: s.karimjonov99@gmail.com

❤️ Mualliflik huquqi
Ushbu loyiha ta’limiy va portfel maqsadlarda foydalanish uchun ochiq.
Tijoriy yoki qayta tarqatish maqsadida ishlatishdan oldin AERLUX bilan bog‘laning.

yaml
Copy code
© 2025 AERLUX — Barcha huquqlar himoyalangan.
