# Arabic product copy: how native products write it

Distilled from `phrasebook.jsonl` (577 rows), `terms.jsonl` (518) and `avoid.jsonl` (55). Modern Standard Arabic (MSA)
for one `ar` locale, Gulf-friendly words. Pilot, November 2026. Nobody who built this reads Arabic: every rule below is
a pattern counted in the sources, and **a native speaker has the last word on every rule**.

Native voices: Talabat, Careem, MBC Shahid, Tamara, Tabby, Uber, HungerStation, Mostaql/Hsoub, Liv, Emirates NBD,
Al Rajhi, Zain, WhatsApp. Platforms: YouTube, Instagram, Facebook, TikTok, Android (AOSP values-ar), Apple (ar-ae),
Google help, Netflix help.

## Gender: the first decision
Arabic marks "you" as masculine or feminine on verbs and suffixes. No product swept ships a gender switch, and only one
feminine string turned up (ENBD 'اقتربتِ من الوصول إلى بطاقتكِ', a women's card flow). Products settle it four ways:

| Strategy | Example | Where |
|---|---|---|
| Verbal noun (masdar), no gender | تسجيل الدخول، إعادة المحاولة، فتح التطبيق، مشاركة، حذف | Android, YouTube, Instagram, TikTok, Facebook buttons |
| Impersonal or passive | حدث خطأ. يُرجى إعادة المحاولة لاحقًا. / تعذّر الاتصال بالخادم / تم حفظ التغييرات. | Google, Meta, Talabat, Shahid errors |
| "You" as a frame word | أمامك 5 دقائق أخرى، يمكنك إلغاء الاشتراك في أي وقت، لديك | Instagram limits, Netflix, Shahid, Apple |
| Masculine imperative | حمّل التطبيق، اطلب الآن، احجز مشوارك، افتح حسابك الآن | Careem, Talabat, Tamara, HungerStation, banks |

Counts (phrasebook register tags): CTAs 110 masculine vs 57 neutral; errors 64 neutral vs 3 masculine; limits and time
36 neutral vs 7; success 17 of 17 neutral. Platforms lean neutral (buttons are masdar); regional brands lean masculine
in marketing.

Rule for an app: masdar for every button, tab, toggle and menu row; impersonal for errors and status; "يمكنك / أمامك"
for sentences about the user; the unvowelled masculine imperative only where a sentence must tell the user to act
("انسخ رابطًا…", Apple's 'افتح تطبيق "الإعدادات".'). Unvowelled past and present ("استخدمت", "تريد") read as default
masculine and every platform uses them; don't add vowels to force a gender. Plural-you ("أهلاً بكم") belongs to welcome
banners only; mixing it with singular on one surface reads careless (Shahid does both, Al Rajhi 'طلبك' + 'طلبكم').

## Buttons and short labels
| English | Arabic | Source |
|---|---|---|
| Log in / Sign in | تسجيل الدخول | Facebook, TikTok, YouTube, Android, Tamara, Uber |
| Log out | تسجيل الخروج | Uber |
| Continue | متابعة | Android, TikTok, Shahid |
| Cancel | إلغاء | everywhere |
| Retry / Try again (button) | إعادة المحاولة | Android Settings, YouTube, TikTok, Shahid |
| Save / Delete / Share | حفظ / حذف / مشاركة | Android, YouTube, TikTok |
| Done | تم | Android, TikTok (YouTube 'تمّ') |
| OK / Got it | حسنًا | Android, YouTube (TikTok 'فهمت ذلك') |
| Not now | ليس الآن | Facebook, TikTok, Android core (YouTube, Android Settings 'لاحقًا') |
| Open app | فتح التطبيق | Facebook, TikTok, Instagram, YouTube |
| Learn more | مزيد من المعلومات / معرفة المزيد | Android / Careem, WhatsApp |
| Turn on / Turn off | تفعيل / إيقاف | Android, YouTube |
| Restore | استعادة; a purchase: استعادة عملية الشراء | Android; Apple support 108096 |
| Skip | تخطي / التخطي | YouTube / Android |
| Download | تنزيل | YouTube, Apple, Google, TikTok, Android |

- Buttons drop the article except where Android keeps it ('السماح', 'التخطي', 'التالي'); pick one style per app.
- Dialog questions open with **"هل تريد …؟"**: "هل تريد حظر هذا المستخدم؟" (Instagram), "هل تريد حذف كل المحتوى الذي
  نزّلته؟" (YouTube), 'هل تريد تفعيل ميزة "توفير البيانات"؟' (Android).
- Progress: **"جارٍ" + masdar**: "جارٍ التنزيل", "جارٍ التحميل..." (YouTube, Facebook, Android).
- Waiting: "في انتظار الاتصال بالإنترنت..." (YouTube).

## Errors, empty screens, success
- Base error: **"حدث خطأ. يُرجى إعادة المحاولة لاحقًا."** (YouTube, Instagram, Android). Short: "حدث خطأ ما." (TikTok,
  Talabat). Soft openers: "عفوًا!" (YouTube, TikTok), "عذرًا،" (Instagram, Shahid).
- Couldn't X: **"تعذّر" + masdar**: "تعذّر إتمام عملية التنزيل." (YouTube), "تعذر الاتصال بالخادم." (Android). A failure
  we own: "لم نتمكن من …" (Talabat), "نواجه مشكلة في تشغيل هذا الفيديو" (Instagram). Short toast: "فشل" + masdar
  ("فشل تحميل الفيديو", TikTok; "فشل طلب الشبكة", Instagram).
- Please: "يُرجى" (Google, vowelled), "يرجى" (Meta, Talabat), "الرجاء" (Shahid). Counts: 14 / 18 / 4.
- Not available: "هذا الفيديو غير متاح" (TikTok), "الفيديو غير متوفّر بلا إنترنت" (YouTube). Full storage: "مساحة تخزين الهاتف
  ممتلئة." (Android).
- Offline: "لا يتوفّر اتصال بالإنترنت." (YouTube), "لا يوجد اتصال بالإنترنت" (TikTok). Back: "تمّت استعادة الاتصال بالإنترنت."
- Empty: **"ستظهر … هنا"**: "ستظهر الفيديوهات التي يتم تنزيلها هنا" (YouTube), "ستظهر الحسابات التي تتابعها هنا" (TikTok).
  "No X yet": "لا توجد مقاطع فيديو حتى الآن" (TikTok), "لم يتمّ تنزيل أي فيديو." (YouTube). No results: "لم يتم العثور على نتائج".
- All caught up: **"لقد اطلعت على كل جديد"** (Instagram).
- Success: **"تم" + masdar** ("تم حفظ التغييرات.", Instagram; "تمّ النسخ إلى الحافظة.", YouTube), with "بنجاح" for weight.
- Can't undo: build from "لا يمكن" + masdar; no sourced exact line.

## Limits and time (Instagram, TikTok, YouTube, Google Digital Wellbeing)
| Situation | Arabic | Source |
|---|---|---|
| Limit reached | لقد وصلت إلى الحد اليومي الخاص بك | Instagram |
| Close it, back tomorrow | حان الوقت لإغلاق Instagram. يمكنك استخدامه مرة أخرى غدًا. | Instagram |
| Minutes left | أمامك 5 دقائق أخرى لاستخدام Instagram اليوم. / يتبقّى $minutes دقيقة | Instagram / YouTube |
| Time's up | انتهى الوقت | YouTube |
| Time used today | لقد استخدمت Instagram لمدة {…} اليوم. | Instagram |
| Break nudge | ألم يحن الوقت لأخذ قسط من الراحة؟ / حان وقت الاستراحة | TikTok / Google |
| Resets | تتمّ إعادة ضبط موقّتات استخدام التطبيقات في منتصف الليل. | Google |
| Resumes tomorrow | سيتم استئناف حدود وقت الاستخدام العادية غدًا. | Instagram |
| Can't use now | لا يمكنك استخدام TikTok أثناء هذه الأوقات | TikTok |
| More time | طلب المزيد من الوقت / إضافة وقت | Instagram / YouTube |

Feature names (reuse the platform's, see `terms.jsonl`): daily limit **الحد اليومي** (Instagram) / حد الوقت اليومي (TikTok);
screen time **مدة الاستخدام** (TikTok), مدة استخدام الجهاز (Apple); sleep hours **ساعات النوم** (TikTok), وضع "وقت النوم"
(Android), وضع النوم (Instagram); Do Not Disturb **عدم الإزعاج**; Focus وضع التركيز (Google) / التركيز (Apple); grayscale
تدرّج الرمادي, "الأبيض والأسود" (Android); picture-in-picture **نافذة ضمن النافذة** (Android Settings) / **صورة داخل صورة**
(Apple, TikTok, Android keywords); sleep timer موقّت إيقاف التشغيل (YouTube); autoplay تشغيل تلقائي (YouTube).

## Pricing and trials
- Trial: **"7 أيام مجانًا"** ("اشترك الآن و استمتع بـ 7 أيام مجانًا", Shahid; tanween normalised).
- Cancel anytime: "يمكنك إلغاء الاشتراك في أي وقت." (Shahid), "يمكنك إلغاء حسابك لدى Netflix في أي وقت."
- No X: **"بدون" + noun** ("بدون أي التزامات" Shahid, "بدون رسوم تأخير" Tamara, "بدون فوائد" Tabby). "بلا" is the
  platform word for offline ("بلا إنترنت", YouTube).
- Once: Apple "يمكنك شراء المشتريات غير الاستهلاكية داخل التطبيق مرة واحدة." Pieces seen: "مرة واحدة" (Apple, Android),
  "دفعة" for a payment (Tabby, Tamara, Shahid 'دفعتك القادمة'). No product sentence for "one payment, not a subscription"
  was found: compose it from these pieces ("دفعة واحدة. بدون اشتراك.") and flag it.
- Charged: "تحصيل الرسوم" ("لن يتم تحصيل رسوم منك", Google Play; "إذا كانت رسوم الشراء قد تم تحصيلها", Apple).
- Restore: "استعادة عملية الشراء" (Apple support). Currency after the number: "24.50 درهم", "19 د.إ", "10 دولار" (Google Play).

## Numerals
Western digits are the consumer default (careem 18/0, tt 268/0, yt 26/0, ig 134/2, tamara 81/0 Western/Arabic-Indic).
Exceptions: Facebook prints counts in Arabic-Indic ("٣٫٣ مليون"), Android mixes three digit sets in one file (never copy
its Persian ۴ ۵ ۶). Use "." for decimals and "," for thousands as YouTube does ("1,839,948,740 مشاهدة"). Format by hand:
locale number APIs can switch to ٠-٩ by region. A field the user types into may receive ٠-٩ from an Arabic keyboard:
don't ask for typed digits.

## Plurals, dual, counted nouns
CLDR gives Arabic six forms and Android and YouTube ship all six (`{videos,plural, =0{0 فيديو}=1{فيديو واحد}two{فيديوهان}
few{# فيديوهات}many{# فيديو}other{# فيديو}}`, YouTube).

| n | Rule | Examples |
|---|---|---|
| 0 | number + singular | 0 فيديو (YouTube), zero{… # خطوة.} (Android) |
| 1 | noun + واحد/واحدة, no digit | دقيقة واحدة، يوم واحد، مقطع ريلز واحد |
| 2 | dual, no digit | دقيقتان، ساعتان، فيديوهان، مقطعا ريلز; after a preposition: دقيقتين، يومين |
| 3–10 | digit + plural | 3 دقائق، 7 أيام، 3 مقاطع ريلز |
| 11–99 | digit + singular (accusative) | 14 دقيقة، 12 ساعة، 11 مقطع ريلز، 120 يومًا (Play) |
| 100+, fractions | digit + singular | 100 يوم، 2.5 سنة |

- A template the code fills without plural forms has two safe frames: **"N من + definite plural"** ("{num_coauthors} من
  الأشخاص الآخرين", Instagram; "١٠ ملايين من المشاهد", Facebook) or a **label colon** ("المدة: $Number$ دقيقة", Shahid).
  The invariant singular ("$minutes دقيقة", YouTube; "{num_minutes} دقيقة", Instagram) is what platforms do, and is
  wrong for 3–10.
- Units: د (minutes, TikTok "غفوة (10 د)"), س (hours), ث (seconds), ي (day, Facebook).
- "And" attaches with no space: "ساعتان و50 دقيقة", "3 ساعات و4 دقائق" (YouTube); also before Latin: "Pay وBox" (Careem).
- Ordinals put the number after the noun: "الحلقة 3", "الموسم 2" (Shahid).

## Punctuation, quotes, tanween
- Arabic comma **،** and question mark **؟** (65 and 36 in the rows; ASCII "?" 0). Full stop unchanged.
- Feature names go in straight double quotes: 'افتح تطبيق "الإعدادات".' (Apple), 'وضع "عدم الإزعاج"' (Android). No «».
- Tanween on the letter before the alif: **غدًا، مجانًا، لاحقًا** (Google, Meta, Apple, TikTok, Netflix; ig 101 vs 4,
  tt 296 vs 18). Shahid, e&, Uber write "غداً"; pick one.
- Slips to avoid: a full stop typed first and stored at the start (".حدّد هدفك", Liv), tatweel "بــ", double tanween "مجاناًً".

## Brands and Latin inside RTL
- Meta, TikTok and YouTube keep brands Latin: "فتح Instagram", "تسجيل الدخول إلى Instagram", "فتح TikTok", "Shorts" (never
  transliterated). Facebook's own UI writes "فيسبوك" ("فتح فيسبوك"), its help titles "Facebook".
- **Reels = "ريلز"** (Instagram, Facebook), counted with مقطع: "مقطع ريلز واحد"، "مقطعا ريلز"، "3 مقاطع ريلز".
- Prepositions before Latin: "لـ iPhone" (Apple), "بـ" likewise; "و" attaches ("وInstagram").
- A line may start with Latin ("Instagram أفضل على التطبيق"): direction must come from the layout, not the first letter.
  Meta and Android insert U+200F around Latin and placeholders; strip when copying, keep when rendering.
- "›" and parentheses are mirrored by the bidi algorithm in RTL; type them as in English.
- Regional brands write their names in Arabic script (كريم، طلبات، تمارا، هنقرستيشن، واتساب).

## Words to settle once
- Download **تنزيل**; on YouTube "تحميل" means *upload* ("يمكنك تحميل الفيديوهات وحفظها"). Loading = "جارٍ التحميل".
- Password: "كلمة السر" (Meta, Talabat, Shahid) and "كلمة المرور" (Google, Apple) are both standard; pick one.
- Feed: no single word. YouTube says "خلاصة" ("خلاصة الصفحة الرئيسية"); Instagram names the page ("الصفحة الرئيسية").
- Post **منشور** (Facebook "إنشاء منشور", Instagram). Suggested **مقترح** ("فيديو مقترح" YouTube, "حسابات مقترحة" TikTok);
  Instagram's feed label is "اقتراحات قد تعجبك". Sponsored **مُموَّل** (Facebook), Ad **إعلان** (Instagram, YouTube).
- Follow **متابعة**; Following: TikTok tab "أتابعه", Instagram "الأشخاص الذين تتابعهم" / menu "المتابعات". For You: TikTok "لك".
- Subscriptions: "الاشتراكات" (Google Play, Apple); YouTube writes "اشتراكاتك" in sentences.
- Watch later **المشاهدة لاحقًا** (YouTube). Library "المكتبة", Queue "قائمة الانتظار", Playback speed "سرعة التشغيل" / "عادية".
- Settings **الإعدادات**; iOS/Android "General" "عام"; App info "معلومات التطبيق"; Open by default "الفتح تلقائيًا"; Open
  supported links "فتح الروابط المتوافقة" (Android Settings).
- Phone: "الهاتف" (MSA) over "الجوال" (Gulf) and "الموبايل".

## Register and dialect
MSA for every platform and bank. Dialect shows up in marketing lines and toasts, never in errors: Saudi "وش حاب تطلب
اليوم؟", "اطلب الحين" (HungerStation), "بس خلّك منتبه!" (Tamara); Gulf/Egyptian "سلتك فاضية!", "اللي بخاطرك، واصلك"
(Talabat). One `ar` locale: MSA throughout, at most one dialect tagline, and Gregorian month names "يناير … ديسمبر"
(Facebook, Google Play), not the Levantine "كانون الثاني".

## Calque tells (see avoid.jsonl)
- **"قم بـ" + masdar** ("قم بالترقية", "قم بإنشاء", "قم بتنزيل": Shahid, TikTok, HungerStation, Liv) = "do the X-ing". Use
  the imperative ("انشر", "حمّل") or the masdar label.
- "الخاص بك" for "your" where a suffix does it ("الحد اليومي الخاص بك" → "حدّك اليومي"); Instagram does it, natives
  write the suffix.
- Hamza slips on imperatives ("إختر", "إدفع"; Talabat), missing hamza ("الان", "ايام"), "الي" for "إلى", Persian ی.
- The singular noun reused for any count ("المدة: $Number$ دقائق" next to "… دقيقة", Shahid) and feminine adjectives
  on masculine nouns.
- Key mix-ups in shipped bundles: "Play" as "لعب", "Phone number" as "رقم الهاتف الأرضي", "My List" as "تفضيل الفيلم".
- Untranslated fragments ("1ي ago") and two names for one feature on one screen.

## Not found (compose and flag)
"Restore purchases" as a button (Apple support has "استعادة عملية الشراء" in prose); a one-time-purchase sentence; iOS's
label "Start PiP Automatically"; Samsung One UI names (Now bar, Lock screen and AOD); a name for "quiet hours" (TikTok's
"ساعات النوم" is the closest feature); "we never see your password"; "data stays on your phone".
