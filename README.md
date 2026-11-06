# Portfolio + Telegram bot orqali so'rovlar

## 1. Telegram bot yaratish
1. Telegramda **@BotFather** -> `/newbot` -> nom va username bering -> **BOT_TOKEN** ni oling.
2. Yangi botingizga kirib **Start** bosing (bo'lmasa bot sizga yoza olmaydi).
3. **@userinfobot** ga `/start` yozing -> u sizning **CHAT_ID** (raqam) ingizni beradi.

## 2. Ishga tushirish (Vercel)
1. Papkani GitHub'ga yuklang -> vercel.com -> Import Project.
2. Settings -> Environment Variables: `BOT_TOKEN` va `CHAT_ID` kiriting -> Redeploy.
3. Tayyor: forma -> `/api/contact` -> Telegram botingiz.

Lokal sinash: `npm i -g vercel`, `.env` yarating (`.env.example` asosida), `vercel dev`.

## Muhim
Tokenni `main.js` yoki `index.html` ichiga YOZMANG: brauzerda hamma ko'ra oladi va botingizni egallab olishi mumkin.

---
## OSPanel (yoki PHP hosting) orqali ishga tushirish
1. Butun `portfolio` papkasini OSPanel loyihalar papkasiga qo'ying (versiyaga qarab `domains` yoki `home`), masalan `portfolio` nomi bilan, va OSPanel'ni ishga tushiring (PHP moduli yoqilgan bo'lsin).
2. `api/config.example.php` faylidan nusxa olib `api/config.php` deb nomlang va `BOT_TOKEN` hamda `CHAT_ID` ni yozing.
3. Brauzerda loyiha manzilini oching (masalan `http://portfolio/`) va formani sinang. Sayt avval `/api/contact` ga, topilmasa `/api/contact.php` ga yuboradi.
4. Internetdagi odamlar ko'rishi uchun sayt domen va ochiq IP/hosting'da turishi kerak. OSPanel o'z kompyuteringizda ishlasa, faqat siz ko'rasiz.

`config.php` ni GitHub'ga yuklamang (`.gitignore` da yozilgan).
