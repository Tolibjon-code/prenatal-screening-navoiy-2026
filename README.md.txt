```markdown
# Генетик Синдромлар Хавф Бахолаш Дастури

Bu repository Streamlit ilovasini o'z ichiga oladi: `app.py` — Genetik sindromlar xavfini hisoblash.

Tez o'rnatish va Streamlit Cloud-ga joylashtirish:

1. Fayllar:
   - app.py — rootda bo‘lsin.
   - requirements.txt — Python paketlari (streamlit, pandas, numpy, plotly).
   - runtime.txt — Python versiyasi (masalan `python-3.11`).
   - .gitignore — (mas’ul fayllar ro‘yxati).
   - streamlit.toml — (ixtiyoriy, konfiguratsiya).

2. GitHub-ga push qilish:
   - `git add .`
   - `git commit -m "Prepare app for Streamlit Cloud"`
   - `git push origin main`

3. Streamlit Cloud-ga deploy:
   - https://streamlit.io/cloud ga kiring va GitHub hisobingizni ulang.
   - "New app" → repository va branch tanlang (masalan `main`) → `app.py` faylini ko‘rsating.
   - Deploy tugmasini bosing.

4. Agar ilova maxfiy ma'lumotlar (API kalitlari) talab qilsa:
   - Streamlit Cloud -> App settings -> Secrets bo‘limida `STORED_SECRETS` sifatida qo‘shing.
   - App ichida `st.secrets["MY_SECRET"]` orqali foydalaning.

Qo‘shimcha tavsiyalar:
- app.py fayli rootda bo‘lishi kerak va `streamlit` ga mos funksiya chaqiriqlari ishlatilgan bo‘lishi lozim.
- `requirements.txt` ichida streamlit versiyasi va boshqa bog‘liqliklar to‘g‘ri pinlangan bo‘lsa, deploy davomida dependency xatoliklari kamayadi.
- Agar muammoga duch kelsangiz, Cloud loglarini tekshiring (Deploy log va App log).

Agar xohlasangiz, men:
- Siz bergan app.py ni repositoryga commit qilish uchun GitHub PR yozib berish taklifini tayyorlayman,
- Yoki requirements.txt ni X versiyalar bilan yangilab beraman,
- yoki deploy qadamlarini bosqichma-bosqich ekranli qo‘llanma qilib yozib beraman.