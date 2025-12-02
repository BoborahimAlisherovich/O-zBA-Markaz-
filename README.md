# Django Project — Installation Guide

Ushbu loyiha Django asosida yaratilgan bo‘lib, quyidagi ko‘rsatmalar yordamida loyihani mahalliy muhitda (local environment) ishga tushirishingiz mumkin.

---

## 📌 1. Repozitoriyani klonlash

```
git clone https://github.com/username/repository-name.git
```


📌 2. Virtual muhit yaratish va faollashtirish


```
python -m venv venv
venv\Scripts\activate
```
MacOS / Linux:
```
python3 -m venv venv
source venv/bin/activate
```
📌 3. Kerakli kutubxonalarni o‘rnatish
Loyihada foydalanilgan barcha paketlar requirements.txt faylida mavjud:

```
pip install -r requirements.txt
```
📌 4. .env yoki settings.py konfiguratsiyasi

📌 5. Ma’lumotlar bazasini yaratish (migratsiyalar)
```
python manage.py makemigrations
```

```
python manage.py migrate
```

📌 6. Superuser (admin) yaratish
```
python manage.py createsuperuser
```
Admin panelga kirish uchun login/parol yarating.

📌 7. Statik fayllarni yig‘ish (production uchun)
```
python manage.py collectstatic
```
📌 8. Loyihani ishga tushirish
```
python manage.py runserver
```
