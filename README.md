# Obsidia - المفكرة الذكية الشخصية للباحث

> "ليست عقلاً بل وعياً بالعقل"

المفكرة الذكية الشخصية للباحث - جزء من منصة إقرأ للتراث الإسلامي

## الفلسفة

Obsidia ليست مجرد تطبيق لتدوين الملاحظات، بل هي طبقة ميتا-معرفية تراقب وتفهم أنماط تفكير الباحث دون التدخل في عملية البحث.

### المبادئ الثلاثة
1. **الشخصية** - لكل باحث مفكرته الخاصة
2. **الامتداد** - تتبع الباحث في رحلته
3. **الاستقلالية** - تعمل بدون اتصال

### الذكاء الصامت
- 90% صامت (يراقب)
- 8% يهمس (ملاحظات خفيفة)
- 2% ينصح (اقتراحات)
- <1% ينبه (تحذيرات مهمة)

## التقنيات

### Backend
- Python 3.11+
- FastAPI
- SQLite مع FTS5
- aiosqlite

### Frontend
- React 18
- Vite
- Tailwind CSS
- React Query
- Zustand
- Recharts

## التشغيل

### Backend
```bash
cd backend
pip install -r requirements.txt
uvicorn main:app --host 0.0.0.0 --port 8001 --reload
```

### Frontend
```bash
cd frontend
npm install
npm run dev
```

## الهيكل

```
obsidia-project/
├── backend/
│   ├── database/
│   │   └── db.py          # SQLite + FTS5
│   ├── models/
│   │   └── schemas.py     # Pydantic models
│   ├── routes/
│   │   ├── notes.py       # CRUD + Wiki-links
│   │   ├── tags.py        # Tags management
│   │   ├── projects.py    # Projects + Questions + Journey
│   │   ├── search.py      # Full-text search
│   │   ├── cognitive.py   # Mirror + Momentum + Patterns
│   │   ├── sync.py        # Local backup + BigQuery
│   │   └── integration.py # 6 Iqra integration points
│   ├── main.py
│   └── requirements.txt
│
├── frontend/
│   ├── src/
│   │   ├── components/    # UI components
│   │   ├── pages/         # App pages
│   │   ├── services/      # API client
│   │   ├── store/         # Zustand store
│   │   └── hooks/         # Custom hooks
│   ├── package.json
│   └── vite.config.js
│
└── README.md
```

## الوظائف المعتمدة (25)

### الأساسيات
- إنشاء/تعديل/حذف الملاحظات
- التاريخ والإصدارات
- البحث الشامل

### التنظيم
- الوسوم والتصنيف
- الربط بين الملاحظات [[wiki-links]]
- المشاريع البحثية

### القنوات
- الكتابة اليدوية
- الاستيراد من الحافظة
- التكامل مع إقرأ

### الذكاء الشخصي
- المرآة المعرفية
- الزخم البحثي
- التقارير الأسبوعية
- اكتشاف الأنماط

### التوثيق
- رحلة المشروع
- الأسئلة والقرارات
- المراجعة المتباعدة

## التكامل مع إقرأ

### من إقرأ إلى المفكرة
1. إرسال اقتباس للملاحظات
2. إرسال نص للتعليق
3. إرسال سؤال للتأمل

### من المفكرة إلى إقرأ
1. عرض في UltraGraph
2. إضافة لـ Zotero Smart
3. إرسال للوكيل

## الترخيص

جزء من منصة إقرأ - جميع الحقوق محفوظة
