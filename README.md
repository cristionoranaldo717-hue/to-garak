# 🎓 EduClub Pro - Premium To'garak Boshqaruv Tizimi

## 📋 Loyiha Haqida

EduClub Pro - bu zamonaviy to'garaklar va o'quv markazlarini boshqarish uchun mo'ljallangan professional veb-platforma. To'liq responsive dizayn, real-time yangilanishlar va zamonaviy UI/UX bilan jihozlangan.

## 🚀 Asosiy Xususiyatlar

### 🎨 Foydalanuvchi Paneli (index.html)
- ✅ Zamonaviy va responsive dizayn
- ✅ To'garaklarga onlayn qo'shilish tizimi
- ✅ Real-time statistika va monitoring
- ✅ Dark/Light mode qo'llab-quvvatlash
- ✅ Smooth animatsiyalar va interaktiv elementlar
- ✅ Kategoriya bo'yicha filtrlash
- ✅ Particle animatsiya background
- ✅ Avtomatik yangilanish (har 3 soniyada)

### 🛡️ Admin Paneli (admin.html)
- ✅ 3 bosqichli xavfsiz kirish tizimi
- ✅ So'rovlarni ko'rish va boshqarish
- ✅ A'zolarni qo'shish/tahrirlash/o'chirish
- ✅ **To'garaklarni zamonaviy modal oyna orqali boshqarish**
- ✅ To'garak statusini boshqarish (Faol/Nofaol)
- ✅ Real-time statistika dashboard
- ✅ CSV/JSON export funksiyalari
- ✅ Qidirish va filtrlash
- ✅ Dark mode qo'llab-quvvatlash
- ✅ Avtomatik yangilanish

## 🔐 Admin Panel Kirish

### Default Ma'lumotlar (O'ZGARTIRING!)

`admin.html` faylida (taxminan 640-643 qatorlar):

```javascript
const ADMIN_CREDENTIALS = {
    email: 'admin@togarak.uz',
    password: '1',              // ⚠️ KUCHLI PAROL O'RNATING!
    secretKey: '1'              // ⚠️ MAXFIY KODNI O'ZGARTIRING!
};
```

### Kirish Jarayoni:
1. `admin.html` sahifasini oching
2. **Email:** admin@togarak.uz
3. **Parol:** 1
4. **Xavfsizlik Kodi:** 1
5. "Kirish" tugmasini bosing

**⚠️ XAVFSIZLIK:** Saytni ishlatishdan oldin bu ma'lumotlarni o'zgartiring!

## 📁 Fayl Tuzilishi

```
📦 EduClub Pro
├── 📄 index.html          # Foydalanuvchi sahifasi
├── 📄 admin.html          # Admin boshqaruv paneli
├── 📄 README.md           # Qo'llanma (siz bu faylni o'qiyapsiz)
├── 📄 ADMIN_INFO.txt      # Admin ma'lumotlari
└── 📄 SAYT MANZILI.txt    # Sayt manzili
```

## 🛠️ Texnologiyalar

| Texnologiya | Versiya | Maqsad |
|------------|---------|--------|
| HTML5 | Latest | Struktura |
| CSS3 | Latest | Styling |
| JavaScript | ES6+ | Funksionallik |
| Tailwind CSS | 3.x | UI Framework |
| Font Awesome | 6.4.0 | Ikonlar |
| Google Fonts | - | Inter, Poppins |
| LocalStorage | - | Ma'lumotlar saqlash |

## 📦 O'rnatish va Ishga Tushirish

### Usul 1: Oddiy Ochish
1. Loyihani yuklab oling
2. `index.html` faylini brauzerda oching
3. Admin panel uchun `admin.html` ni oching

### Usul 2: Live Server (VS Code)
1. VS Code da loyihani oching
2. Live Server extension o'rnating
3. `index.html` da o'ng tugma → "Open with Live Server"

### Usul 3: Python HTTP Server
```bash
# Loyiha papkasida
python -m http.server 8000

# Keyin brauzerda:
# http://localhost:8000/index.html
# http://localhost:8000/admin.html
```

## 🎯 Qanday Ishlaydi?

### To'garak Qo'shish (Admin)
1. Admin panelga kiring
2. "To'garaklar" bo'limiga o'ting
3. "Yangi To'garak" tugmasini bosing
4. **Modal oyna ochiladi:**
   - To'garak nomini kiriting
   - A'zolar sonini kiriting
   - Dars jadvalini kiriting
   - Status tanlang (Faol/Nofaol)
5. "Saqlash" tugmasini bosing
6. ✅ To'garak darhol qo'shiladi va localStorage ga saqlanadi

### To'garak Tahrirlash (Admin)
1. To'garak kartochkasida "Tahrirlash" tugmasini bosing
2. Modal oynada ma'lumotlarni o'zgartiring
3. "Saqlash" tugmasini bosing
4. ✅ O'zgarishlar darhol saqlanadi

### Foydalanuvchi Tomonidan
1. `index.html` sahifasini oching
2. To'garaklar avtomatik ko'rinadi (har 3 soniyada yangilanadi)
3. Faqat **Faol** statusdagi to'garaklar ko'rsatiladi
4. "A'zo bo'lish" tugmasini bosing
5. Formani to'ldiring va yuboring
6. Admin tasdiqlashini kuting

## 🔧 Sozlash va Xavfsizlik

### 1. Admin Ma'lumotlarini O'zgartirish

`admin.html` faylini oching va quyidagi qismni toping:

```javascript
const ADMIN_CREDENTIALS = {
    email: 'sizning@email.uz',           // O'z emailingiz
    password: 'Kuchli_Parol_2024!@#',    // Kuchli parol
    secretKey: 'Maxfiy-Kod-XYZ-2024'     // Maxfiy kod
};
```

### 2. Xavfsizlik Choralari
- ✅ 3 bosqichli autentifikatsiya
- ✅ 5 marta noto'g'ri urinishdan keyin 5 daqiqa bloklash
- ✅ Session boshqaruvi (localStorage)
- ⚠️ **Muhim:** Production uchun backend kerak!

### 3. Ma'lumotlarni Tozalash

Agar muammo bo'lsa, brauzer console da:

```javascript
// Barcha ma'lumotlarni tozalash
localStorage.clear();

// Yoki faqat ma'lum bir ma'lumotni:
localStorage.removeItem('circlesData');
localStorage.removeItem('joinRequests');
localStorage.removeItem('approvedMembers');
```

## 📊 Funksiyalar Ro'yxati

### Admin Panel Funksiyalari:

| Funksiya | Tavsif | Status |
|----------|--------|--------|
| Dashboard | Umumiy statistika va ko'rsatkichlar | ✅ |
| So'rovlar | Yangi so'rovlarni ko'rish va tasdiqlash | ✅ |
| A'zolar | A'zolar ro'yxatini boshqarish | ✅ |
| To'garaklar | Modal oyna orqali CRUD operatsiyalar | ✅ |
| Tahlillar | Grafiklar va statistika | ✅ |
| Sozlamalar | Dark mode, bildirishnomalar | ✅ |
| Export | CSV va JSON formatda export | ✅ |
| Qidirish | A'zolarni qidirish | ✅ |

### Foydalanuvchi Funksiyalari:

| Funksiya | Tavsif | Status |
|----------|--------|--------|
| To'garaklar | Barcha faol to'garaklarni ko'rish | ✅ |
| Filtrlash | Kategoriya bo'yicha filtrlash | ✅ |
| Ariza | To'garakka ariza berish | ✅ |
| Statistika | Real-time statistika | ✅ |
| Dark Mode | Tungi rejim | ✅ |
| Responsive | Barcha qurilmalarda ishlash | ✅ |

## 🐛 Muammolarni Hal Qilish

### ❌ Admin panelga kira olmasam?

**Sabab 1:** Noto'g'ri ma'lumotlar
```
✅ Yechim: Email, parol va secret key ni tekshiring
```

**Sabab 2:** Bloklangan
```
✅ Yechim: 5 daqiqa kuting yoki localStorage.clear() bajaring
```

**Sabab 3:** Brauzer muammosi
```
✅ Yechim: Boshqa brauzerda sinab ko'ring
```

### ❌ To'garak qo'shilmayapti?

**Sabab:** Modal oyna ochilmayapti
```
✅ Yechim: 
1. Brauzer console ni oching (F12)
2. Xatolarni tekshiring
3. Sahifani yangilang (Ctrl+F5)
```

### ❌ Foydalanuvchi sahifasida to'garaklar ko'rinmayapti?

**Sabab:** localStorage bo'sh
```
✅ Yechim:
1. Admin panelda kamida 1 ta to'garak qo'shing
2. Status "Faol" ekanligini tekshiring
3. Foydalanuvchi sahifasini yangilang
```

### ❌ Ma'lumotlar yo'qoldi?

**Sabab:** LocalStorage tozalangan
```
✅ Yechim:
1. Admin panelda qaytadan to'garaklar qo'shing
2. Backup oling (Export tugmasi)
3. Brauzer cache ni tozalamang
```

## 📱 Qo'llab-quvvatlash

### Brauzerlar:
- ✅ Chrome 90+
- ✅ Firefox 88+
- ✅ Safari 14+
- ✅ Edge 90+

### Qurilmalar:
- ✅ Desktop (1920x1080 va yuqori)
- ✅ Laptop (1366x768 va yuqori)
- ✅ Tablet (768x1024)
- ✅ Mobile (320x568 va yuqori)

## 🔄 Yangilanishlar

### v1.2.0 (Joriy) - 2024
- ✅ To'garak qo'shish/tahrirlash modal oynasi
- ✅ Form validatsiyasi
- ✅ Escape tugmasi bilan modal yopish
- ✅ Bo'sh holatlar uchun xabarlar
- ✅ Real-time statistika yangilanishi
- ✅ Faqat faol to'garaklarni ko'rsatish
- ✅ Dizayn yaxshilandi

### v1.1.0 - 2024
- ✅ LocalStorage integratsiyasi
- ✅ Admin va foydalanuvchi sinxronizatsiyasi
- ✅ Avtomatik yangilanish (3 soniya)

### v1.0.0 - 2024
- ✅ Asosiy funksiyalar
- ✅ Admin panel
- ✅ Xavfsizlik tizimi

## 📝 Litsenziya

Bu loyiha ta'lim va shaxsiy maqsadlar uchun yaratilgan. Erkin foydalanishingiz mumkin.

## ⚠️ Muhim Eslatmalar

1. **Production uchun:** Backend (Node.js, PHP, Python) va database (MySQL, MongoDB) kerak
2. **Xavfsizlik:** Admin ma'lumotlarini o'zgartiring
3. **Backup:** Muntazam ravishda ma'lumotlarni export qiling
4. **Testing:** Ishga tushirishdan oldin to'liq test qiling

## 👨‍💻 Yordam va Qo'llab-quvvatlash

Agar savollaringiz bo'lsa:
1. README.md ni diqqat bilan o'qing
2. ADMIN_INFO.txt faylini tekshiring
3. Brauzer console da xatolarni ko'ring

---

**🎉 Muvaffaqiyatli ishlatishingizni tilaymiz!**

EduClub Pro Development Team © 2024
