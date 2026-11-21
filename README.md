# nativecopy

**How real products say it, in other languages.** A phrasebook of short UI and marketing strings that people wrote
natively in Russian, Azerbaijani and Turkish (Turkish is a pilot), lined up with English and tagged by situation.

AI models translate words well and meaning badly: "Back to top" comes out as a word-for-word calque, the register
flips between formal and casual, and a feature gets a name no local user has ever seen. This repo gives a writer
(or an agent) the way well-written local products already say the same thing.

## What's in it

```
<lang>/phrasebook.jsonl   aligned rows: native text, English, situation, register, product, source url, why it's good
<lang>/terms.jsonl        feature names as big platforms show them (reuse the name, not the phrasing)
<lang>/avoid.jsonl        calques, stiff and machine-translated forms, kept as bad examples
<lang>/GUIDE.md           rules distilled from the rows (register, button verbs, errors, limits, time)
SOURCES.md                every source tried, its voice score and why it was kept or dropped
```

One row:

```json
{"lang":"ru","text":"…","en":"…","situation":"empty_done","register":"ty","product":"…","url":"…","note":"…"}
```

`situation` is one of: cta, headline, onboarding, settings, limit_time, empty_done, error, success, notification,
privacy_security, pricing, help, misc. `register` is ty / vy (ru), sen / siz (az, tr), or impersonal.

## How rows get in

1. Sources are picked for a native editorial voice (local companies writing in their own language, global products
   known for good localization) and scored 1–5 on how native they read. Low scorers are dropped and listed.
2. Agents fetch public pages (JavaScript pages in a headless browser with a fresh profile, never logged in) and pull
   short strings, paired with the English page where one exists. Locale files that sites ship publicly give real
   key-by-key pairs.
3. Every row is checked word for word against the saved raw page; anything not found is dropped.
4. Every row is reviewed and tiered by hand; a native speaker has the last word.

Only short phrases are quoted, each with its source URL. Product names and strings belong to their owners.

## License

Code: MIT. The curated data (selection, tags, notes, guides): CC BY 4.0. Quoted strings: see NOTICE.
