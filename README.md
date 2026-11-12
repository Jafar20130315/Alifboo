<div align="center">

# 🔤 Alifboo

**Uzbek Alphabet Converter API**

[![Version](https://img.shields.io/badge/version-1.1.0-blue.svg)](https://github.com/jafaras/alifboo)
[![Cloudflare Workers](https://img.shields.io/badge/Cloudflare-Workers-orange.svg)](https://workers.cloudflare.com)
[![License](https://img.shields.io/badge/license-MIT-green.svg)](LICENSE)

Конвертирует узбекский латинский текст из старого написания (O'/G'/Sh/Ch) в новый официальный алфавит (Ö/Ğ/Ş/Ç)

[Демо](https://alifboo.jafaras.uz) • [Документация](#документация) • [Примеры](#примеры-кода)

</div>

---

## 📖 Описание

**Alifboo** — это быстрый и надёжный API для конвертации узбекского текста. Работает на edge-серверах Cloudflare по всему миру, обеспечивая минимальную задержку ответа (< 100 мс из любой точки мира).

### Возможности

- ✅ Конвертация одной строки
- ✅ Batch-конвертация (до 500 строк за раз)
- ✅ Конвертация HTML с сохранением тегов
- ✅ Rate limiting для защиты от злоупотреблений
- ✅ CORS для использования из браузера
- ✅ Живое демо на главной странице

---

## 🚀 Быстрый старт

### 1. Конвертация одной строки

```bash
curl -X POST https://alifboo.jafaras.uz/convert \
  -H "Content-Type: application/json" \
  -d '{"text": "O'\''zbekiston Respublikasi"}'
