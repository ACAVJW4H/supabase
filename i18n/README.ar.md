<div style="direction: rtl;" dir="rtl">

<p align="center">
  <img width="300" src="https://raw.githubusercontent.com/supabase/supabase/master/web/static/supabase-light-rounded-corner-background.svg"/>
</p>

---

# Supabase

[Supabase](https://supabase.com)هو بديل مفتوح المصدر لـ(Firebase). نحن نبني ميزات (Firebase) باستخدام أدوات مفتوحة المصدر عالية الجودة تستخدمها الشركات.

- [x] قاعدة بيانات (Postgres) مستضافة.
- [x] اشتراكات الوقت الفعلي.
- [x] المصادقة والترخيص.
- [x] واجهات برمجة التطبيقات التي يتم إنشاؤها تلقائيا.
- [x] لوحة الإدارة.
- [x] التخزين.
- [ ] الدوال (مفردها دالّة).

## الشرح

للحصول على الشرح الكامل، قم بزيارة [supabase.io/docs](https://supabase.com/docs).

## المجتمع والدعم

- [منتدى المجتمع](https://github.com/supabase/supabase/discussions). الأفضل لـ: المساعدة في البناء، والنقاش حول أفضل ممارسات قاعدة البيانات.
- [مشاكل GitHub](https://github.com/supabase/supabase/issues). الأفضل لـ: المشاكل والأخطاء التي تواجهها عند استخدامك لـ(Supabase).
- [دعم البريد الإلكتروني](https://supabase.com/docs/support#business-support). الأفضل لـ: مشاكل مع قاعدة بياناتك أو البنية التحتية.
- [ديسكورد](https://discord.supabase.com/). الأفضل لـ: مشاركة التطبيقات الخاصه بك وقضاء بعض الوقت مع المجتمع.

## الحالة

- [x] طور الألفا: نحن نختبر Supabase مع مجموعة مغلقة من العملاء
- [x] طور الألفا العام: يمكن لأي شخص الاشتراك في [app.supabase.io] (https://app.supabase.io). لكن تحلى بالصبر ، فهناك بعض العقد الصغيرة.
- [x] طور البيتا العام: مستقر بدرجة كافية لمعظم حالات الاستخدام غير المتعلقة بالمؤسسات
- [ ] الطور العام: جاهز للإنتاج

نحن حاليًا في طور البيتا العام. شاهد "إصدارات" هذا المستودع لتلقي إخطارات بالتحديثات الرئيسية.

<kbd><img src="https://gitcdn.link/repo/supabase/supabase/master/web/static/watch-repo.gif" alt="Watch this repo"/></kbd>

## كيف يعمل (Supabase)؟

Supabase عبارة عن مجموعة من الأدوات مفتوحة المصدر. نحن نبني ميزات (Firebase) باستخدام أدوات مفتوحة المصدر عالية الجودة تستخدمها الشركات. إذا كانت الأدوات والمجتمعات موجودة ، باستخدام MIT أو Apache 2 أو ترخيص مفتوح مكافئ ، فسنستخدم هذه الأداة وندعمها. إذا لم تكن الأداة موجودة ، فإننا نبنيها ونفتح مصدرها بأنفسنا. (Supabase) ليس تعيين 1 إلى 1 لـ(Firebase). هدفنا هو منح المطورين تجربة مطور تشبه (Firebase) باستخدام أدوات مفتوحة المصدر.

**الهيكلة الحالية**

(supabase) هي [منصة مستضافة](https://app.supabase.io), يمكنك التسجيل والبدأ باستخدامها دون الحاجة لتثبيت أي شئ. يمكنك أيضا [استضافتها ذاتيا](https://supabase.com/docs/guides/self-hosting) و [تطويرها داخليا](https://supabase.com/docs/guides/local-development).

![Architecture](https://supabase.com/docs/assets/images/supabase-architecture-9050a7317e9ec7efb7807f5194122e48.png)

- [PostgreSQL](https://www.postgresql.org/) هي قاعدة بيانات قائمة على العلاقات الشيئية مع ٣٠ سنة من التطوير النشط التي اكسبتها سمعة وموثقية قوية وتمتاز بالمتانة والأداء.
- [Realtime](https://github.com/supabase/realtime)
- [PostgREST](http://postgrest.org/)
- [Storage](https://github.com/supabase/storage-api)
- [postgres-meta](https://github.com/supabase/postgres-meta)
- [GoTrue](https://github.com/netlify/gotrue)
- [Kong](https://github.com/Kong/kong)

#### المكتبات

مكتباتنا معيارية. كل مكتبة فرعية هي تطبيق مستقل لنظام خارجي واحد. هذه إحدى الطرق التي ندعم بها الأدوات الحالية.

- **`supabase-{lang}`**: يجمع المكتبات ويضيف الإثراء.
  - `postgrest-{lang}`: مكتبة العميل للعمل مع [PostgREST] (https://github.com/postgrest/postgrest)
  - `realtime-{lang}`: مكتبة العميل للعمل مع [Realtime] (https://github.com/supabase/realtime)
  - `gotrue-{lang}`: مكتبة العميل للعمل مع [GoTrue] (https://github.com/netlify/gotrue)

| المستودع              | الرسمي                                           | المجتمع                                                                                                                                                                                                                    |
| --------------------- | ------------------------------------------------ | -------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| **`supabase-{lang}`** | [`JS`](https://github.com/supabase/supabase-js)  | [`C#`](https://github.com/supabase/supabase-csharp) \| [`Dart`](https://github.com/supabase/supabase-dart) \| [`Python`](https://github.com/supabase/supabase-py) \| `Rust`                                                |
| `postgrest-{lang}`    | [`JS`](https://github.com/supabase/postgrest-js) | [`C#`](https://github.com/supabase/postgrest-csharp) \| [`Dart`](https://github.com/supabase/postgrest-dart) \| [`Python`](https://github.com/supabase/postgrest-py) \| [`Rust`](https://github.com/supabase/postgrest-rs) |
| `realtime-{lang}`     | [`JS`](https://github.com/supabase/realtime-js)  | [`C#`](https://github.com/supabase/realtime-csharp) \| [`Dart`](https://github.com/supabase/realtime-dart) \| [`Python`](https://github.com/supabase/realtime-py) \| `Rust`                                                |
| `gotrue-{lang}`       | [`JS`](https://github.com/supabase/gotrue-js)    | [`C#`](https://github.com/supabase/gotrue-csharp) \| [`Dart`](https://github.com/supabase/gotrue-dart) \| [`Python`](https://github.com/supabase/gotrue-py) \| `Rust`                                                      |

## الترجمات

- [قائمة الترجمات](/i18n/languages.md) <!--- Keep only this -->

## الرعاة

[![New Sponsor](https://user-images.githubusercontent.com/10214025/90518111-e74bbb00-e198-11ea-8f88-c9e3c1aa4b5b.png)](https://github.com/sponsors/supabase)

</div>
