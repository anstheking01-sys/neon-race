NEON RACE — إعداد سريع

1) افتح app.js ببرنامج Notepad.
2) ابحث عن السطر SUPABASE_URL واستبدل النص PASTE_YOUR_SUPABASE_PROJECT_URL_HERE برابط مشروعك فقط، مثل:
   https://YOURPROJECT.supabase.co
   لا تضع /rest/v1 في نهاية الرابط.
3) استبدل PASTE_YOUR_SUPABASE_PUBLISHABLE_KEY_HERE بمفتاح Publishable من Supabase.
   لا تستخدم service_role أو أي secret key في موقع الويب.
4) احفظ الملف.
5) ارفع كل ملفات المجلد إلى مستودع GitHub ثم Settings > Pages واختر النشر من الفرع الرئيسي والجذر /root.
6) في Supabase > Authentication > URL Configuration أضف رابط موقع GitHub Pages إلى Site URL وRedirect URLs. إذا كان تأكيد البريد مفعّلًا، أكّد البريد قبل تسجيل الدخول.

قاعدة البيانات: استخدم SQL الذي نفذته سابقًا لإنشاء race_profiles وrace_results.

ملاحظات:
- هذه نسخة أولية قابلة للتطوير. اللعبة تعمل في المتصفح؛ التسجيل ولوحة النتائج يحتاجان اتصال Supabase.
- لا تضع أبدًا service_role/secret key في app.js.
- وقت السباق محسوب بالمتصفح ويمكن التلاعب به؛ لا تعتبره نظامًا تنافسيًا آمنًا قبل إضافة تحقق من جهة الخادم.
