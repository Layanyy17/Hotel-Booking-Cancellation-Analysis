# دليل استكمال رفع ملفات المشروع على GitHub

أنشئ المستودع بنجاح، وتم رفع README وملفات التوثيق الأساسية.

## الملفات التي تحتاج رفعًا

- `hotel_bookings_Analysis.xlsx` — ملف Excel الأصلي بحجم يقارب **68.4 MiB** (أكبر من حد الرفع العادي عبر متصفح GitHub، وهو 25 MiB للملف الواحد).
- `assets/dashboard_overview.png` — صورة الداشبورد الرئيسي.
- `assets/risk_deep_dive.png` — صورة صفحة Risk Deep Dive.

الملفات الثلاثة موجودة داخل حزمة `Hotel_Booking_GitHub_Ready.zip` التي تم تجهيزها في المحادثة.

## رفع الصور من المتصفح

1. افتحي المستودع: https://github.com/Layanyy17/Hotel-Booking-Cancellation-Analysis
2. اختاري `Add file` ثم `Upload files`.
3. اسحبي مجلد `assets` من الحزمة بعد فك ضغط ZIP، مع المحافظة على أسماء الملفات ومسار المجلد.
4. أكملي `Commit changes`.

## رفع ملف Excel باستخدام GitHub Desktop

1. نزّلي GitHub Desktop من https://desktop.github.com ثم سجّلي دخولك إلى حساب GitHub.
2. اختاري `File > Clone repository` وحددي `Layanyy17/Hotel-Booking-Cancellation-Analysis`.
3. افتحي المجلد المحلي للمستودع وانسخي بداخله ملف `hotel_bookings_Analysis.xlsx`.
4. ارجعي إلى GitHub Desktop، اكتبي رسالة commit مثل `Add interactive Excel analysis workbook`، ثم اختاري `Commit to main` وبعدها `Push origin`.
5. تأكدي من ظهور الملف في المستودع.

## تنبيه قبل النشر العام

تأكدي أن مصدر مجموعة البيانات يسمح بإعادة نشر ملف البيانات كاملًا. إن لم تكن رخصته واضحة، اكتفي برفع صور الداشبورد وREADME ونتائج التحليل إلى أن تتحققي من صلاحية نشر البيانات.

## ملاحظة

GitHub يعرض ملف Excel كملف للتنزيل، وليس داشبورد تفاعليًا مباشرًا؛ التفاعل والفلاتر يكونان من خلال فتح الملف على Microsoft Excel لسطح المكتب.
