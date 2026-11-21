# Sources

Every source tried (November 2026: pilot, then round 2 with JavaScript-rendered pages, new industries and Turkish), how native its voice reads (1–5), and where its rows went.
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

| Source | Voice | Register | Used as | Note |
|---|---|---|---|---|
| Spotify (premium, support) | 5 | sen | phrase | Best subscription and cancel wording; rewrites, not translates |
| fizy | 4.5 | sen | phrase | en is a gloss |
| Turkcell, BiP | 4 | siz (sen in ads) | phrase | The English is the translated side |
| ininal, Enpara, Garanti BBVA, Vodafone, Türk Telekom, İş Bankası | 4 | siz | phrase (few) | Vodafone mixes sen and siz on one page |
| Storytel | 3.5 | sen marketing, mixed bundle | row by row | 891 keys paired with en; register flips in billing copy |
| Android (AOSP strings) | 4 | siz | term | Apache-2.0 |
| Google Digital Wellbeing, YouTube Help | 3 | siz | term | Labelled AI-translated |
| Instagram Help | 3 | siz, sen for teens | row by row | Passive nominal titles, 'anında ilet bildirimi' |
| Not reached | | | | Getir, Yemeksepeti, Trendyol, Hepsiburada, n11, sahibinden, Armut, BiTaksi, Pegasus, THY (403 or empty); Papara, Exxen (consent wall); Max TR, BluTV, Gain, Martı (empty or not Turkish UI) |

## Licences
No commercial source states a licence for its interface text. The repo quotes only short strings, each with its URL.
Android/AOSP strings are Apache-2.0 (attribution in NOTICE). MediaWiki (GPL) and Firefox (MPL) strings were read but
left out of the data, since their licences don't mix with CC BY 4.0.

The `en` field is the product's own English line where `en_source` is `page`. Localizers often rewrite rather than
translate, so the two can differ in detail; that difference is usually what the row teaches.
