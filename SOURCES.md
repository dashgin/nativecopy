# Sources

Every source tried in the pilot (November 2026), how native its voice reads (1–5), and where its rows went.
`phrase` rows are models to write from; `term` rows are platform UI names to reuse but not to imitate in phrasing;
`avoid` rows are kept as bad examples. Tiers are set row by row, not per source. Every row was checked word for word against the fetched page; 66 that could not
be found were dropped. State strings (errors, limits, empty screens) come from locale files the sites ship publicly,
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
| Checked and skipped as вы | | | | Duolingo ru, Steam, Pinterest, Canva, Snapchat, Aviasales, Discord (ты only in jokes) |
| Not reached | | | | T-Bank (certificate error), Avito (refused), Instagram help and TikTok support (JavaScript), Duolingo (JavaScript) |

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
| Not reached / no az | | | | Duolingo, Netflix, Zoom, Opera (no az); Booking, Uber, Canva (blocked); Meta and Instagram help (JavaScript); Microsoft Terminology (licence unverified, not harvested) |

## Licences
No commercial source states a licence for its interface text. The repo quotes only short strings, each with its URL.
Android/AOSP strings are Apache-2.0 (attribution in NOTICE). MediaWiki (GPL) and Firefox (MPL) strings were read but
left out of the data, since their licences don't mix with CC BY 4.0.

The `en` field is the product's own English line where `en_source` is `page`. Localizers often rewrite rather than
translate, so the two can differ in detail; that difference is usually what the row teaches.
