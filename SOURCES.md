# Sources

Every source tried (November 2026: pilot, then round 2 with JavaScript-rendered pages, new industries, Turkish and Georgian), how native its voice reads (1–5), and where its rows went.
`phrase` rows are models to write from; `term` rows are platform UI names to reuse but not to imitate in phrasing;
`avoid` rows are kept as bad examples. Tiers are set row by row, not per source. Every row was checked word for word against the saved raw page (round 2 rendered JavaScript pages in a headless
browser with a fresh profile); rows that could not be found were dropped. State strings (errors, limits, empty screens) come from locale files the sites ship publicly,
looked up by key.

## Russian

| Source | Voice | Register | Used as | Note |
|---|---|---|---|---|
| Telegram (translations platform, site) | 5 | Вы (capitalised) | phrase | Rewrites instead of translating; strings keyed to English |
| Spotify support | 5 | вы | phrase | Best subscription and failed-payment wording |
| Skyeng (app, FAQ) | 5 | ты in app, вы on web | phrase | Only ru exists; English is a gloss |
| Yandex (Go, 360, Plus, Music, Browser, Alice, Kinopoisk) | 4 | вы / infinitive | phrase | Drops "ваш", plain verbs |
| Ozon (App Store) | 3 | | phrase (few) | |
| Apple Support / iPhone guide | 4 / 3 | вы | term | Names good, guide phrasing stiff |
| Google: Android, Digital Wellbeing, YouTube help | 4 | вы | term | Pages carry an AI-translation notice |
| TikTok newsroom | 2.5 | | avoid | Press-release tone; support site needs JavaScript |
| Kaspersky Safe Kids | 2 | | avoid | Translated from English, genitive chains |
| Lingualeo | 4 | ты | phrase | Whole dictionary inlined in the page, ru and en by key; the ru is the original |
| Иви (ivi.ru) | 4 | ты | phrase | Public i18n file with readable keys; en is a gloss |
| Делимобиль, Yota, КИОН | 4–5 | ты | phrase (few) | Page bundles; en is a gloss |
| Checked for ты, all вы | | | | Duolingo ru, Steam, Pinterest, Canva, Snapchat, Aviasales, Discord (ты only in jokes) |
| Duolingo (web app locale bundles) | 5 | вы | phrase | Same keys in ru and en; localises rather than translates («Повторение — мать учения») |
| Avito Support | 5 | вы, questions in the user's «я» | phrase | Plain, honest limits («Ускорить не получится — нужно подождать.»); en is a gloss |
| START | 4.5 | вы | phrase | Best failed-payment and cancel-reason wording; en is a gloss |
| Пикабу | 4.5 | вы | phrase | Humour in empty and error states; en is a gloss |
| hh.ru | 4 | вы | phrase | ~4,500 keys inlined; limits, autorenew, cancel; en is a gloss |
| Островок | 4–4.5 | вы | phrase | Keyed ru/en bundle, real pairs |
| ОК (Одноклассники) | 4 | вы | phrase | Keyed ru/en dictionary; ru is the original |
| 2ГИС, Папа Джонс, Облако Mail, Дзен, ВкусВилл, Wink, Туту, Т-Банк help | 3.5–4 | вы (ты in loyalty, game, a few prompts) | phrase | en is a gloss |
| Нетология | 3–3.5 | вы | phrase (few) | |
| Госуслуги | 2 | | avoid | Only the error page reached; officialese |
| TikTok Support | 3 | вы | term | Machine-localised; feature names only |
| Instagram, Facebook Help | 3–4 | вы | term | Machine-localised; one feature has two names |
| Not reached | | | | T-Bank main site (certificate error), avito.ru (429), Сбер, Альфа, ВТБ, РЖД, Rutube, Wildberries, Okko, Самокат, Купер, Мегамаркет, Учи.ру, Звук (blocked or empty); VK (dictionary only via its API) |

## Azerbaijani

| Source | Voice | Register | Used as | Note |
|---|---|---|---|---|
| Yelo Bank | 5 | sən | phrase | Casual, light slang; its English is the weaker translation |
| Birbank / Kapital Bank | 4–5 | sən (siz in news, support) | phrase | |
| m10 | 4 | sən | phrase | FAQ slips into stiff passives |
| Bolt, Bolt Food | 4 | sən (siz for merchants) | phrase | |
| Wolt | 4 | siz | phrase | |
| Bakcell, Azercell, Nar | 4 | sən | phrase | Written in az first; their English is translated |
| tap.az, Birmarket | 4 | | phrase (few) | |
| Spotify | 3.5 | siz + sən mixed | phrase | Best trial and cancel wording |
| WhatsApp site | 3–4 | siz | phrase | Some machine errors ("Dizayna görə…") |
| ABB | 3 | siz | phrase (few) | English calques, button/body register mismatch |
| Android (AOSP strings) | 4 | siz | term | Apache-2.0 |
| Google Account, Translate, Play | 3.5–4 | siz | term | Play has machine errors |
| YouTube web UI | 3.5 | siz | term | "Vaxt bitdi" good; Unmute = "Susdurmayın" (wrong) |
| TikTok | 3–3.5 | | term | Screen-time names; writes the feed as "lent" |
| MediaWiki | 3.5 | | excluded | GPL-2.0-or-later does not mix with CC BY data; read, not included |
| Firefox (Pontoon) | 2.5 | | excluded | MPL-2.0, same reason; Turkish pasted as az in places |
| Airbnb | 3.5 marketing, 1 help | | term / avoid | Help articles are labelled auto-translated |
| Leobank | 3 | | row by row | Reads translated from Russian; natural rows kept ("Hesabı böl"), calques in avoid |
| Yango | 3 marketing, 2 help | mixed | row by row | Native lines kept ("Gününüz rahat keçsin"); Russian officialese in avoid |
| YouTube Help | 2 | | term / avoid | Labelled AI-translated; typos. Clean button labels kept as terms only |
| Telegram az | 2 | | excluded | Public site shows only unapproved crowd suggestions |
| PASHA Bank | 3 | siz | row by row | Business page only |
| Bakcell web (state strings) | 4.5 | sən | phrase | Locale JSON in the page; the most consistent sən voice |
| Birbank web, PASHA, Baku Metro | 3.5–4 | | phrase / term | Errors, waits, empty states |
| Wolt web (state strings) | 3–4 | siz (some sən) | row by row | ~3.7k az/en pairs inlined; translators differ |
| tap.az, Bina.az, ABB | 3–3.5 | siz | row by row | Russian-first; 'hələ ki', 'Hal hazırda sizin' in avoid |
| Lalafo | 2.5 | | row by row | English left in az strings, typos; worst rows in avoid |
| iTicket | 4 | siz, sən in gifting | phrase | 1,199 az/en keys in locale chunks |
| myGov (my.gov.az) | 4 new strings, 2–3 legacy | siz | row by row | ~380 az/en keys; chatbot errors are the best state strings found |
| PASHA Sığorta | 4–5 | sən | phrase | ~640 az/en keys |
| Unibank, Rabitəbank, Expressbank, Araz | 4 | sən | phrase | |
| Baku Electronics | 3 | sən + siz mixed | row by row | 'Sizin hal-hazırda …' calques in avoid |
| AccessBank, Huawei, Samsung, Irshad, Azərpoçt | 3–4 | | phrase (few) | |
| ASAN, DOST, BakuBus, Atəşgah, PASHA Life | 2–3 | | avoid (mostly) | Officialese, Turkish words |
| TikTok Support az | 2.5 | siz | term / avoid | Labelled AI-translated |
| Instagram, Facebook Help az | 1 | | avoid / term | Mostly English with az words spliced in |
| Not reached / no az | | | | Duolingo, Netflix, Zoom, Opera (no az); Booking, Uber, Canva, Kontakt, AZAL, ADY, CinemaPlus, Oxu, Bank Respublika, Ultel, Citynet, Trendyol, e-gov, e-Təbib, Azərişıq, Azərsu (blocked or unreachable); Microsoft Terminology (licence unverified, not harvested) |

## Turkish

Round 2, November 2026 (pilot of 113 phrases and 30 terms, now 519 phrases, 384 terms, 40 avoid). Key-paired sources first: Instagram, TikTok, YouTube, Duolingo and Android ship locale tables, so the `en` column is the product's own English. Every new row was checked word for word against the saved raw page (HTML entities, `\uXXXX` and Android `\'` escapes decoded; whitespace collapsed); `en_source: gloss` marks the rows whose English is ours, not on the page. JavaScript pages and Facebook were rendered in headless Chrome with a throwaway profile, never logged in.

| Source | Voice | Register | Used as | Note |
|---|---|---|---|---|
| Spotify (premium, support) | 5 | sen | phrase | Best subscription and cancel wording; rewrites, not translates. Round 2 added the cancel and refund help pages paired with `us` English |
| fizy | 4.5 | sen | phrase | en is a gloss |
| Instagram web (tr_TR JS bundles, ~2.7k module-keyed string pairs with en_US) | 4 | sen, a few siz stragglers (ads panel, "İzlediğiniz") | phrase, term | Meta's own time-management copy ("Süre kontrolü", "Uyku modu"), app banners, errors; header "Instagram Uygulamada Daha İyi Bir Deneyim Sunar" is Title Case; template bugs (`{username}'(n)in`) went to avoid |
| TikTok web (rehydration data, 2.4k key pairs) | 4 | siz | phrase, term | Screen-time, sleep and break reminders; "Sizin İçin", "Takip ediliyor / Takipte / Takip Edilen" on one site; "Delay" translated as "Gecikme" went to avoid |
| YouTube (web, mobile web, Premium page; ytcfg key tables, ~680 pairs) | 4 | siz | term, phrase | "Süre doldu" (sleep timer), offline and download states, "Uygulamayı Aç"; Premium page has the trial and cancel lines; small grammar slips in avoid |
| Duolingo web (tr and en string chunks, 3.8k id pairs) | 4 | sen, siz in billing | phrase | "Süren doldu!", reminders, "Ücretsiz denememi başlat", "tek seferlik", purchase confirmed and failed; register flips in payment errors |
| Facebook web (login, Watch, Groups, Help Center, mobile web; tr_TR and en_US) | 3.5 | sen, siz in business help | term, phrase | "Katıl", "Reels", "Tanıyor Olabileceğin Kişiler", "Sponsorlu" (help search), mobile install banner; logged-in feed strings not public |
| Apple Support (iPhone User Guide tr-tr, iOS 27) | 4 | siz | term | "Ekran Süresi", "Süre İzinleri", "Ekran Süresi Zamanlaması", "Odak"; Apple says "aygıt" and "parola" |
| Netflix Help Center | 4 | siz | phrase | Cancel and download pages paired with en; officialese in places ("tahsil edilmeyecektir") |
| Android (AOSP strings: Settings, SystemUI, framework, PermissionController, MediaProvider) | 4 | siz | term, phrase | Apache-2.0; picture-in-picture, storage, permissions, notifications, DND; abbreviations ("Uyglr") and "Kablosuz" in avoid |
| Paycell, Martı, TOD, Pinterest TR, WhatsApp TR | 3.5 | sen (Paycell, TOD), siz (Pinterest, WhatsApp) | phrase (few) | English is a gloss |
| Turkcell, BiP | 4 | siz (sen in ads) | phrase | The English is the translated side |
| ininal, Enpara, Garanti BBVA, Vodafone, Türk Telekom, İş Bankası | 4 | siz | phrase (few) | Vodafone mixes sen and siz on one page |
| Storytel | 3.5 | sen marketing, mixed bundle | row by row | 891 keys paired with en; register flips in billing copy |
| Google Digital Wellbeing, YouTube Help | 3 | siz | term | Labelled AI-translated |
| Instagram Help | 3 | siz, sen for teens | row by row | Passive nominal titles, 'anında ilet bildirimi' |
| Not reached | | | | Getir (405), Yemeksepeti (Cloudflare geo ban), Trendyol (empty), Hepsiburada ("Güvenlik" wall), n11 (Cloudflare), Papara (Cloudflare challenge), BiTaksi (403), sahibinden, Armut, Pegasus, THY, Exxen (consent wall), Max TR, BluTV, Gain (empty or not Turkish UI); Telegram translations (crowd suggestions only), WhatsApp FAQ articles (400 without a browser), Facebook feed labels "Sponsorlu / Önerilen / Gruba Katıl" as UI (only in logged-in app), Spotify app strings (not public), Microsoft Terminology (licence unverified, not harvested) |

## Georgian

Round: November 2026. Georgian-first consumer sites rarely ship a public locale file, so most rows from them have an English gloss; key-paired sources (Wolt, YouTube, Android) carry the product's own English. Every row was checked word for word against the saved raw page (placeholders such as `$minutes` are kept as written). Facebook pages were rendered in headless Chrome with a throwaway profile; Facebook's logged-in UI strings (Sponsored, Suggested for you, Join group, Follow) are not on any public page and were not found.

| Source | Voice | Register | Used as | Note |
|---|---|---|---|---|
| Wolt (web app, ka and en locale keys) | 3.5 | თქვენ (-ეთ) mostly, sen in a few strings | phrase | ~3.7k key pairs inlined in the page; translators differ (four different "Done" buttons), typos and English left over; those went to avoid |
| YouTube (web and mobile web, ka and en bundles) | 4 | თქვენ (-ეთ) in sentences, bare nouns on buttons | term, phrase | ~270 desktop and ~220 mobile key pairs; "Shorts" stays Latin; counts read "ნახვა" (views), "გამომწერი" (subscribers), "უყურებს" (watching) |
| YouTube Help | 2.5 | თქვენ | term (names), avoid | Labelled AI-translated; English titles left in the sidebar; break and bedtime reminder names kept |
| Facebook (login, sign-up, Watch, Help Center, ka_GE) | 3.5 | თქვენ, sen imperatives in some help titles | term, avoid | Paired with the en_US pages; Reels = "ფირები", Threads = "ჯაჭვები"; Help Center mixes Georgian and English titles |
| Facebook ka_GE JS bundles (ads manager strings) | 3 | | term | Georgian only, no English in the file; names of placements (Reels, feed, Stories) |
| Instagram | 2 | | term (few), avoid | The site does not serve Georgian; Help Center and the Play listing do ("ფირი", "რგოლები", "ისტორიები") |
| TikTok | | | not served | Language picker lists ქართული, but web and support pages stay English; only the Play tagline is Georgian |
| Google Play listings of Instagram, Facebook, YouTube, TikTok (ka) | 2.5–3 | თქვენ, sen mixed in | phrase, avoid | Machine-flavoured: Reels as "რგოლები" and "ბორბლები" (wheels), "Home- ზე" with a stray space |
| Android (AOSP strings: Settings, SettingsLib, SystemUI, framework, PackageInstaller, Contacts) | 3.5–4 | თქვენ (-ეთ), nouns on buttons | term, phrase | Apache-2.0; truncated labels ("სინქრ", "გაფართოებ.") and wrong senses ("Power" = "ძალა") in avoid |
| Google Search, Account, Play store (ka) | 4 | თქვენ | term | Cleanest short labels; Search voice errors are good state strings |
| Bolt (ka-ge) | 4 | sen, one -ეთ banner | phrase | Bare imperatives, spelled-out "შენი"; the best marketing voice found |
| Cellfie | 4 | sen | phrase | "საჩუქრები გელოდება!"; comma decimals in prices |
| Magti | 3.5 | sen | phrase | |
| Glovo | 3 | sen and -ეთ mixed | phrase (few) | |
| Yandex Go (ka_ge) | 3 | თქვენ | phrase (few) | Russian-style words ("გეოპოზიცია", "ავტორიზაცია") |
| TBC Pay, Credo Bank, Liberty Bank | 3.5 | თქვენ, sen in one TBC Pay headline | phrase (few) | Mostly navigation; fee lines and 404 wording kept |
| SilkGO (myvideo.ge, silktv.ge), TKT.ge, Extra.ge, ss.ge, Adjarabet, GWP, Silknet | 3–4 | sen in marketing, თქვენ in service text | phrase (few) | Navigation heavy; headlines and relative-time lines kept |
| WhatsApp site (ka) | | | term (2) | Only "ჩამოტვირთვა" and "შესვლა" are Georgian |
| Fetched, not used | | | | Zoommer, Tegeta, Lelo, Imedi (news headlines), Silknet and Magti navigation beyond the lines above |
| Not reached or no Georgian | | | | Telegram translations platform (strings need a login), Spotify and Netflix (no Georgian UI in the Georgian market), TBC Bank main site (empty shell), Bank of Georgia (empty or nav only), Space Bank (connection failed), myauto.ge, myhome.ge, vendoo.ge (bot wall, 403), Mtavari (empty render), Magti TV and Beeline (empty), Google Digital Wellbeing help (served in English or not found), Yandex Go main (no Georgian strings), Europebet |

## Arabic

Round 3 (November 2026). Target is Modern Standard Arabic as written for Gulf, Levant and Egypt consumer products;
dialect is flagged in the row notes. Every row is a verbatim string from a saved raw page (curl with a desktop or mobile
user agent, or headless Chrome with a fresh profile, never logged in). Where a site ships ar and en strings under the
same key (Talabat, Shahid, YouTube, TikTok, Android), `en` is the product's own English line. The rest carry a gloss
(`en_source: gloss`). Registers are `masc` (2nd person masculine, imperative or 'you can' frame), `fem`, `plural`,
`neutral` (masdar labels, impersonal passives, 'يرجى').

| Source | Voice | Register | Used as | Note |
|---|---|---|---|---|
| Careem (ae, sa) | 4.5 | masc | phrase | Plain masculine imperatives, Gulf 'مشوار', Western digits |
| Tamara | 4.5 | masc, Saudi dialect | phrase | 'وش', 'الحين', 'عشان': the most native marketing voice found; one case slip in avoid |
| Uber (ae) | 4 | masc | phrase | Every verb fully vowelled; mixes 'كود QR' and 'رمز' |
| HungerStation | 4 | masc, Saudi dialect | phrase | 'وش حاب تطلب اليوم؟', 'اطلب الحين', 'المقاضي' |
| Tabby | 4 | masc, some dialect | phrase | Percent sign position flips ('%5' vs '10%') |
| Mostaql, Hsoub | 4 | masc | phrase | Clean MSA; a few hamza drops ('الان', 'انشئ') |
| Netflix Help | 4 | masc, neutral | phrase | Best cancel-anytime wording ('يمكنك إلغاء حسابك ... في أي وقت') |
| Talabat web (ar/en bundles in the page) | 3–4 | neutral, masc, Gulf dialect | phrase / avoid | 800+ key-paired strings; dialect lines ('سلتك فاضية') beside hamza slips, Persian letters, key mix-ups |
| MBC Shahid web (ar/en bundles) | 3 | masc, plural | phrase / avoid | Trial, cancel-anytime, payment errors; 'قم ب' + masdar calques, doubled tanween, mismatched keys |
| Liv, Emirates NBD | 3.5 | masc, one fem, one plural | phrase | Banking tone; leading full stops from RTL punctuation, a vowelled feminine 'بطاقتكِ' |
| Al Rajhi Bank | 3.5 | masc, Saudi dialect in promos | phrase (few) | Dialect promo next to formal body; 'طلبك' + 'طلبكم' in one sentence |
| WhatsApp | 3.5 | neutral (masdar headlines) | phrase / term | Formal MSA, no imperatives in headlines |
| Zain KSA | 3 | masc | phrase (few) | Menu-heavy; 'إدفع' hamza slip in avoid |
| YouTube (mobile web, desktop, Help) | 4 | neutral, masc | term / phrase | ~400 keys paired with en; 'يُرجى', 'تعذّر', time and offline states; Levant month names |
| Instagram web bundles | 3.5 | neutral, masc | phrase / term | Screen-time and limit wall strings (best find); 'الخاص بك' for 'your'; no Sponsored label logged out |
| Facebook (web, mobile web, Ad Library, Help) | 3.5 | neutral | term | Arabic-Indic digits; 'مُموَّل' only from the Ad Library; 'Facebook' and 'فيسبوك' both used |
| TikTok web (ar/en keyed) | 3 | masc, neutral | term / phrase / avoid | Screen-time copy is strong; tab 'أتابعه' and 'قم ب' calques |
| Android AOSP (Settings, SystemUI, core) | 3.5–4 | neutral, masc | term | Apache-2.0. Inconsistent across files ('حسنًا' vs 'موافق'); mixed digit sets |
| Apple Support (ar-ae), apple.com privacy | 4.5 | masc | phrase / term | 'مدة استخدام الجهاز', 'التركيز'; consistent 'اضغط' (touch) vs 'انقر' (Mac) |
| Google Digital Wellbeing and Play help | 4 | masc, neutral | term / phrase | 'موقّتات استخدام التطبيقات', 'وضع التركيز'; clean imperatives |
| Fetched, not used | | | | stc, e&, du (menu text only), Spotify (support site is English), Duolingo welcome page (ar strings sit in a lazy chunk, not extracted) |
| Not reached | | | | Anghami (406 and empty render), Noon and Namshi (403), Jahez (challenge page), stc pay (timeout), Telegram translations (crowd suggestions only, 17 Arabic characters), WhatsApp FAQ and privacy (400), logged-in feed labels (Instagram 'Sponsored' and 'Suggested posts', Facebook feed 'Sponsored' and 'People you may know' as a card title) |

## Licences
No commercial source states a licence for its interface text. The repo quotes only short strings, each with its URL.
Android/AOSP strings are Apache-2.0 (attribution in NOTICE). MediaWiki (GPL) and Firefox (MPL) strings were read but
left out of the data, since their licences don't mix with CC BY 4.0.

The `en` field is the product's own English line where `en_source` is `page`. Localizers often rewrite rather than
translate, so the two can differ in detail; that difference is usually what the row teaches.
