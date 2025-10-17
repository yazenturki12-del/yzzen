# Discord Music Bot

بوت ديسكورد بسيط لتشغيل الموسيقى من YouTube (عن طريق البحث أو رابط).

الميزات
- تشغيل أغاني من YouTube عبر اسم أو رابط.
- قائمة انتظار (queue).
- أوامر بالعربية والإنجليزية.
- رسائل مدمجة (Embeds) لعرض معلومات الأغاني.

المتطلبات
- Node.js (مستحسن v20+)
- توكن بوت من Discord Developer Portal
- أذونات البوت في السيرفر: Send Messages, Embed Links, Connect, Speak, Read Message History

كيفية الإعداد والتشغيل محليًا
1. استنساخ المستودع:
   git clone https://github.com/yazenturki12-del/yzzen.git
   cd yzzen

2. تثبيت التبعيات:
   npm install

3. إضافة ملف المتغيرات البيئية .env (أنشئ ملفًا جديدًا في جذر المشروع):
   DISCORD_TOKEN=your-discord-bot-token-here

4. تشغيل البوت:
   npm start
   # أو
   node index.js

تشغيل على Replit
- انسخ المشروع إلى Replit، ثم في Secrets أو Environment variables أضف المفتاح DISCORD_TOKEN بقيمة توكن البوت.
- اضغط Run.

أوامر البوت (موجز)
- !ش <اسم أو رابط> — تشغيل أغنية من YouTube
- !س — تخطي الأغنية الحالية
- !ق — إيقاف التشغيل والخروج من القناة الصوتية
- !قائمة — عرض قائمة الانتظار
- !مساعدة — عرض قائمة الأوامر

ملاحظات مهمة
- فعّل Message Content Intent في Discord Developer Portal (Bot → Privileged Gateway Intents).
- تأكد من أن البوت لديه أذونات الصوت (Connect, Speak) وأنك داخل قناة صوتية عند طلب تشغيل أغنية.
- لا ترفع ملف .env علنًا أو إلى مستودع عام.
