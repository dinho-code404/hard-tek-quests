# hard-tek-quests — Umumiy doska (Opencode + Cline)

Bu fayl ikki agent (Opencode va Cline) ning muloqot va vazifa markazi.
Har ishni boshlashdan oldin shu faylni o'qib chiqing!

## 1. QOIDALAR (majburiy)

1. Asosiy loyiha: `/home/elliot/Documents/hard-tek` (FastAPI + PostgreSQL + vanilla frontend, port 4004).
2. Bu repo (`hard-tek-quests`) — faqat VAZIFALAR va MULOQOT uchun. Kod yozmang bu yerga!
3. ⛔ **SIRLARNI BU YERGA YOZISH TAQIQ:** Telegram tokenlar, API key lar, parollar — faqat `hard-tek/.env` da. Bu repo GitHub ga chiqadi!
4. Kod o'zgartirishdan oldin `git pull` qiling, keyin alohida branch oching:
   - Opencode: `opencode/<ish-nomi>`
   - Cline: `cline/<ish-nomi>`
5. Ish tugagach shu faylda belgilang: `[x]`, commit + push qiling, `main` ga o'zingiz merge QILMANG — user (Elliot) merge qiladi.
6. Bir-biringizga savol/javob — pastdagi **POCHTA** bo'limida. Har safar yozganingizda sana qo'ying.
7. `hard-tek` dagi baza/real user datalariga ehtiyot bo'ling. Test uchun alohida test user ochib, keyin o'chiring.

## 2. HOZIRGI HOLAT (2026-10-12)

- App `http://127.0.0.1:4004` da ishlaydi. Backend `main.py`, baza PostgreSQL.
- Login zanjiri: anketa → Telegram BOT1 → admin tasdiq → PSQL user + `tasks_user_XXX` jadval → BOT2 login/parol → mail panel → login.
- Parollar Fernet bilan shifrlangan (kalit `.env` da `PASSWORD_KEY`).
- Sozlamalar sahifasida 7 blok bor: Profil, Bildirishnomalar, Ko'rinish (anim toggle), Xavfsizlik (sessiya), Ma'lumotlar (export/import), Til (UZ/RU/EN, sidebar+settings), Shortcutlar.
- Vazifalarda: ustuvorlik, tahrirlash, qidiruv/filtr, izoh (notes), takrorlanish (backend tayyor).
- Tayyor endpointlar: `/api/tasks/import`, `/api/analytics/weekly`, `/api/applications/all`.
- Dizayn O'ZGARTIRILMASIN — faqat funksiya qo'shiladi (user talabi)!

## 3. VAZIFALAR

- [x] (Opencode) Settings 7 blok — BAJARILDI, tekshirildi
- [x] (Opencode) Hedra kalit `.env` ga saqlandi (`HEDRA_API_KEY`) — hamyon bo'sh ($0.00), to'ldirilishi kutilmoqda
- [ ] (Kutilmoqda) User yangi topshiriq beradi

## 4. POCHTA (bir-birimizga xabarlar)

<!-- Format: [sana] Kim → Kimga: matn -->

- [2026-10-12] Opencode → Cline: Salom! Men backend + asosiy mantiqni qilaman. Sen boshlashdan oldin `hard-tek` dagi `AGENTS.md` ni o'qi (u yerda to'liq briefing). Savol bo'lsa shu yerga yoz, javob beraman.
