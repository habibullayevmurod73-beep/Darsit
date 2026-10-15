# Korxonani avtomatlashtirish — o'quv ilovasi

Tarozi, kamera, server, 1C va sun'iy intellekt bo'yicha 22 bo'lim, 111 dars, testlar,
avtomatik tekshiriladigan mashqlar, laboratoriya, loyihalar va sertifikat.

Ilova bitta `index.html` faylida ishlaydi. Telefonda «Bosh ekranga qo'shish» orqali
oddiy ilova kabi o'rnatiladi va internetsiz ham ochiladi.

## Fayllar

| Fayl | Vazifasi |
|------|----------|
| `index.html` | Ilovaning o'zi: barcha darslar, testlar va kod |
| `manifest.json` | Telefonga ilova sifatida o'rnatish uchun ma'lumot |
| `sw.js` | Oflayn ishlash (service worker) |
| `icon-*.png` | Ilova belgisi |
| `.nojekyll` | GitHub Pages fayllarni o'zgartirmasligi uchun |

## GitHub Pages'ga joylash (brauzer orqali, dasturlarsiz)

1. github.com saytida akkaunt oching yoki kiring.
2. Yuqori o'ngdagi **+** → **New repository**.
3. Nomini yozing, masalan `avtomatlashtirish`. **Public** ni tanlang va **Create repository** ni bosing.
4. Ochilgan sahifada **uploading an existing file** havolasini bosing.
5. Shu papkadagi **barcha fayllarni** sudrab tashlang (`.nojekyll` ham).
   Kompyuteringiz yashirin fayllarni ko'rsatmasa, `.nojekyll` siz ham ishlaydi.
6. Pastda **Commit changes** ni bosing.
7. Repozitoriyda **Settings** → chap menyudagi **Pages**.
8. **Source**: *Deploy from a branch*, **Branch**: `main`, papka: `/ (root)` → **Save**.
9. 1–2 daqiqadan keyin sahifaning tepasida manzil chiqadi:
   `https://FOYDALANUVCHI-NOMINGIZ.github.io/avtomatlashtirish/`

## Git orqali joylash (terminal bilan)

```bash
cd avtomatlashtirish
git init
git add .
git commit -m "O'quv ilovasi"
git branch -M main
git remote add origin https://github.com/FOYDALANUVCHI-NOMINGIZ/avtomatlashtirish.git
git push -u origin main
```

Keyin yuqoridagi 7–9-qadamlar bilan GitHub Pages'ni yoqing.

## Telefonga ilova sifatida o'rnatish

- **iPhone (Safari):** manzilni oching → pastdagi «Ulashish» belgisi → **Bosh ekranga qo'shish**.
- **Android (Chrome):** manzilni oching → yuqori o'ngdagi ⋮ → **Ilovani o'rnatish** yoki **Bosh ekranga qo'shish**.

## Yangilash

1. Yangi `index.html` ni repozitoriyga yuklang (eski fayl ustidan).
2. `sw.js` ichida `VERSION` ni o'zgartiring (`v1` → `v2`) — shunda telefonlardagi eski nusxa yangilanadi.

## Progress haqida

Progress (darslar, testlar, qaydlar) har bir foydalanuvchining o'z brauzerida saqlanadi.
Boshqa qurilmaga o'tkazish uchun: **Reja** → **Zaxira** → «Progress kodini nusxalash».
