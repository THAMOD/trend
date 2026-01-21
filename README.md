# Trend — Bilingual E‑commerce

React + Tailwind frontend with Express + JSON file storage backend for a bilingual (EN/AR with RTL) clothing store.

## 📍 الروابط وأرقام المنافذ (Ports & URLs)

### السيرفر (Backend):
- **البورت**: `8080` (يمكن تغييره عبر متغير `PORT` في `.env`)
- **الرابط**: `http://localhost:8080`
- **API Health Check**: `http://localhost:8080/api/health`
- **API Products**: `http://localhost:8080/api/products`

### الواجهة (Frontend):
- **البورت**: `8080`
- **الرابط**: `http://localhost:8080`
- **الصفحة الرئيسية**: `http://localhost:8080/`
- **لوحة الأدمن**: `http://localhost:8080/admin`

## 🚀 Quick start

### 1) تثبيت المكتبات
```bash
cd server && npm install
cd ../client && npm install
```

### 2) إعداد ملفات البيئة

**السيرفر** (`server/.env`):
```env
PORT=8080
ADMIN_TOKEN=your-secret-token-here
```

**الواجهة** (`client/.env` - اختياري):
```env
VITE_API_URL=http://localhost:8080
VITE_WA_NUMBER=201234567890
```

> ملاحظة: إذا لم تنشئ `client/.env`، سيستخدم الافتراضي `http://localhost:8080`

### 3) تشغيل السيرفرات

**نافذة CMD الأولى** (السيرفر):
```bash
cd server
npm start
```
يجب أن ترى: `Trend API running on http://localhost:8080`

**نافذة CMD الثانية** (الواجهة):
```bash
cd client
npm run dev
```
سيظهر رابط مثل: `http://localhost:8080`

## ✨ Features
- Full English/Arabic UI toggle, RTL-aware layout.
- Modern deep-blue / gold theme with Tailwind.
- Product catalog and details page with size/color/quantity selection.
- Cart drawer with WhatsApp order message (prefills items and total).
- Admin dashboard to add products securely via `x-admin-token`.
- Local JSON file storage (`server/data.json`) for products persistence.

