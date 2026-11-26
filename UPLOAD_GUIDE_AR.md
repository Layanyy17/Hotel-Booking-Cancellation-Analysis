# رفع آخر ملفات المشروع إلى GitHub

**تمّ:** إنشاء المستودع العام، ورفع README النهائي، وملخص البيانات المرئي، وملاحظات LinkedIn، وتوثيق نتائج Sensitivity Analysis.

**المتبقي في GitHub:** النسخة النهائية من ملف Excel وصورتان فقط. وضعت هذه الملفات **بنفس الأسماء والمجلدات الصحيحة** داخل ملف ZIP قابل للتنزيل من محادثة ChatGPT:

- hotel_bookings_Analysis.xlsx — ملف المستخدم النهائي، 17 ورقة، 43.6 MB
- assets/dashboard_overview.png — صورة لوحة Dashboard بعد اقتصاص القوائم
- assets/risk_deep_dive.png — صورة لوحة Risk Deep Dive بعد اقتصاص القوائم

## ارفعي الملفات الثلاثة دفعة واحدة — GitHub Desktop

1. نزّلي ملف **Hotel_Booking_Final_GitHub_Package.zip** من المحادثة وفكي الضغط.
2. افتحي **GitHub Desktop** وسجلي الدخول بحساب **Layanyy17**.
3. اختاري **File → Clone Repository** وحددي المستودع **Layanyy17/Hotel-Booking-Cancellation-Analysis**.
4. افتحي **مجلد المستودع** على الكمبيوتر.
5. انسخي ملف Excel ومجلد **assets** من المجلد الناتج عن فك ZIP إلى مجلد المستودع (دون نسخ ملف التعليمات).
6. في GitHub Desktop اكتبي رسالة commit: **Add final Excel workbook and dashboard screenshots**.
7. اضغطي **Commit to main** ثم **Push origin**.

رابط المستودع:
https://github.com/Layanyy17/Hotel-Booking-Cancellation-Analysis

**لماذا GitHub Desktop؟** ملف Excel حجمه 43.6 MB، وهو أكبر من حد الرفع العادي من متصفح GitHub (25 MiB)، لكنه أقل من حد ملفات Git المعتاد (100 MiB).

**تنبيه نشر:** قبل رفع سجلات الحجوزات في مستودع عام، تأكدي أن مصدر مجموعة البيانات يسمح بإعادة نشرها. GitHub لا يعرض داشبورد Excel تفاعليًا داخل المتصفح؛ يجب تنزيله وفتحه في Microsoft Excel.
