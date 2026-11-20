# ClipPro لأندرويد

هذا مشروع Android يحوّل ملف ClipPro HTML إلى تطبيق Android باستخدام WebView، ويضم ملف المحرر الأصلي داخل التطبيق.

## إنشاء APK تلقائياً

1. فك ضغط مجلد المشروع.
2. أنشئ مستودعاً جديداً على GitHub وارفع جميع ملفات هذا المجلد إليه.
3. افتح تبويب **Actions** في المستودع.
4. اختر **Build ClipPro APK** ثم **Run workflow**.
5. بعد نجاح البناء، افتح نتيجة التشغيل ونزّل ملف **ClipPro-APK** من قسم Artifacts.
6. فك ضغط الملف الناتج، ثم ثبّت `app-debug.apk` على هاتف Android.

## البناء محلياً

تحتاج Android Studio أو Android SDK (منصة 35) وJDK 17 وGradle 8.9. من جذر المشروع شغّل:

```bash
gradle assembleDebug
```

ستجد الملف في:

`app/build/outputs/apk/debug/app-debug.apk`

## ملاحظة

هذا غلاف Android لصفحة HTML الأصلية. بعض وظائف المتصفح/الذكاء الاصطناعي تحتاج اتصال إنترنت ومفاتيح API الخاصة بها، كما قد تختلف بعض واجهات الويب حسب إصدار Android System WebView.
