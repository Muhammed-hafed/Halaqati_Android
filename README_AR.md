# تطبيق حلقتي Android

هذه حزمة Android Studio جاهزة لتطبيق **حلقتي**. التطبيق يفتح ملف `index.html` داخل WebView، لذلك يعمل كتطبيق عادي على أندرويد ويحافظ على نفس الواجهة والبيانات المحلية.

## طريقة استخراج APK

1. ثبّت Android Studio على الكمبيوتر.
2. فك ضغط هذا الملف.
3. افتح مجلد `HalaqatiAndroid` من Android Studio.
4. انتظر حتى ينتهي Gradle Sync.
5. من القائمة اختر:
   `Build` → `Build Bundle(s) / APK(s)` → `Build APK(s)`
6. بعد الانتهاء اضغط `locate` وستجد ملف APK عادةً في:
   `app/build/outputs/apk/debug/app-debug.apk`

## ملاحظات

- اسم التطبيق: حلقتي
- الحزمة: `com.halqa.app`
- نوع التطبيق: Android WebView App
- ملف التطبيق الأساسي موجود في: `app/src/main/assets/index.html`
- زر النسخ الاحتياطي يحفظ ملف JSON في مجلد التنزيلات داخل الهاتف.
- زر الاستيراد يفتح مدير الملفات لاختيار نسخة JSON.

## لتحديث التطبيق لاحقًا

استبدل الملف:
`app/src/main/assets/index.html`
بنسخة HTML أحدث، ثم ابنِ APK من جديد.

---

## البناء بدون Android Studio

أضفت لك طريقة ثانية لا تحتاج Android Studio. افتح الملف:
`README_BUILD_WITHOUT_ANDROID_STUDIO_AR.md`

الفكرة: ترفع المشروع إلى GitHub، ثم تبني GitHub Actions ملف APK تلقائيًا في السحابة.
