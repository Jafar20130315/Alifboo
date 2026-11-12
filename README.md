<div align="center">

# 🔤 Alifboo

O'zbek lotin alifbosini yangi rasmiy alifboga o'tkazish API'si

[![Version](https://img.shields.io/badge/versiya-1.1.0-blue.svg)]()
[![License](https://img.shields.io/badge/litsenziya-MIT-green.svg)]()

[QO'LLANMA](https://alifboo.jafaras.uz) • [Hujjatlar](#qanday-ishlaydi) • [Misollar](#kod-misollari)

</div>

---

## Alifboo nima?

Alifboo — bu oddiy va tez ishlaydigan API. Eski yozuvdagi o'zbek lotin matnini (O', G', Sh, Ch) yangi rasmiy alifboga (Ö, Ğ, Ş, Ç) o'tkazib beradi.

Masalan:

| Kirish | Natija |
|--------|--------|
| `O'zbekiston` | `Özbekiston` |
| `G'afur G'ulom` | `Ğafur Ğulom` |
| `Shavkat Mirziyoyev` | `Şavkat Mirziyoyev` |
| `Chimyon` | `Çimyon` |

Sayt, ilova yoki botingizda o'zbek matnini yangi alifboga o'tkazish kerak bo'lsa — Alifboo shu ishni qiladi. Bir HTTP so'rov yuborasiz, tayyor natijani olasiz.

---

## Qanday ishlaydi

API'ga matn yuborasiz, u sizga konvertatsiya qilingan matnni qaytaradi. Hammasi shu.

**So'rov:**
```json
POST https://alifboo.jafaras.uz/convert
Content-Type: application/json
{
"text": "O'zbekiston Respublikasi"
}
```

**Javob:**
```json
{
  "success": true,
  "original": "O'zbekiston Respublikasi",
  "converted": "Özbekiston Respublikasi"
}


