Agri System — بناء تطبيق أندرويد (APK) حقيقي
==========================================

هذا المجلد يبني ملف APK على خوادم GitHub (مجاناً)، فيطلب التطبيق الأذونات من نظام الهاتف مباشرة
(الميكروفون، الكاميرا، الموقع) مثل أي تطبيق عادي.

الخطوات من الهاتف (Termux):
1) أنشئ مستودعاً جديداً على GitHub باسم  agri-system-apk
2) في Termux:
     unzip agri-system-apk-kit.zip -d agri-system-apk
     cd agri-system-apk
     git init
     git add -A
     git commit -m "apk kit"
     git branch -M main
     git remote add origin https://github.com/USERNAME/agri-system-apk.git
     git push -u origin main
3) افتح المستودع على GitHub ← تبويب Actions ← سير العمل "Build APK" ← انتظر 5-10 دقائق حتى يصبح أخضر.
4) افتح آخر تشغيل ← في الأسفل Artifacts ← نزّل Agri-System-APK ← فك الضغط ← ثبّت app-debug.apk
   (اسمح بتثبيت التطبيقات من هذا المصدر عندما يطلب الهاتف).
5) عند أول فتح يطلب التطبيق الميكروفون ثم الكاميرا ثم الموقع.

ملاحظة: الملف الموقّع بمفتاح debug مناسب للاستخدام الشخصي. لتحديث التطبيق: عدّل www/ وادفع التغيير، ثم نزّل APK جديداً.
