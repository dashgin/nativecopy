# Azerbaijani product copy: how native products write it

Distilled from `phrasebook.jsonl` (native sources), `terms.jsonl` (platform UI names) and `avoid.jsonl` (calques).
Pilot, November 2026. A native speaker has the last word on every rule.

## Register
- Consumer apps speak **sən** with a bare imperative: "Balansını artır", "Başla", "abunə ol", "Daxil ol" (Bakcell, Nar,
  Birbank, m10, Yelo, Bolt). Merchant, B2B, legal text and forms use **siz** ("Kuryer tərəfdaşı olun", Wolt).
- Pick one per surface and keep it. Mixing on one page reads careless: Yango has "Tətbiqi yüklə" and "Tətbiqi yükləyin"
  side by side.
- The pronoun drops; "your" lives in the suffix: "millərinlə", "gəlirini", "Nömrənlə bağlı", not "sənin milləriniz".

## Buttons and short labels
- Verb, bare: Başla, Davam et, Ləğv et, Təsdiq et, Daxil ol, Ətraflı öyrən, X-i endir / yüklə.
- Join = **"X-li ol" / "X-a qoşul"** ("Azercell-li ol", "Nar-a qoşul"), never "Qoşulun bizə".
- Sign in = **Daxil ol(un)**; "Giriş" works as a noun label. "Giriş et" (Spotify, Airbnb) looks like a Turkish-style
  calque; awaiting a native-speaker check.
- Logins / credentials = **giriş məlumatları**, never "girişlər".
- Dialog questions take **-ilsin?**: "Bu ödəniş üsulu silinsin?", "Saxlanılmamış dəyişikliklər ləğv edilsin?".
  A negative setting takes -məsin ("göndərilməsin").

## Stock phrases natives reach for
| English idea | Native az | Source |
|---|---|---|
| at your fingertips / one tap | bir toxunuşda, bir toxunuşla | Bolt, banks |
| no branch visit, no queue | filiala / banka gəlmədən, növbə gözləmədən | Birbank, Yelo |
| spend the way you like | ürəyincə xərclə | Birbank |
| choose what suits you | özünə ən rahat olanı seç | Nar |
| tap, tap, done | Bir neçə klik, vəssalam! | Bolt Food |
| let us handle it | X bizlikdir ("Çatdırılma bizlikdir") | Bolt Food |
| we do the heavy lifting | bütün ağır işləri öz üzərimizə götürürük | Wolt |
| don't fall for scams | dələduzların tələsinə düşmə | m10 |
| got questions? | Sualların var? | m10 |
| cancel anytime | istənilən vaxt ləğv edin / et | Spotify |
| top up | balansını artır | Bakcell, Nar |
| free | pulsuz (shops, apps), ödənişsiz (Google, WhatsApp) | |

## Errors, limits, empty screens
- Base error: **"Xəta baş verdi. Yenidən cəhd et(in)."** Warmer: "Oyy, nəsə xəta baş verdi!" (Wolt).
- A failure we own takes **-ə bilmədik**: "eSIM QR kodunu yükləyə bilmədik. Yenidən cəhd et." (Bakcell),
  "Sifarişinizi yerləşdirə bilmədik" (Wolt). "… mümkün olmadı / deyil" is the cooler, impersonal form.
- Time's up: **"Vaxtın bitdi"** (Bakcell). A wait: "Yenidən göndərmək üçün {time} gözləyin" (Birbank).
- A limit: "SMS göndərmə limiti bitdi", "limitə çatdınız"; a lockout says when it lifts: "Növbəti cəhd bir saatdan sonra
  aktiv olacaq."
- A conflict gives the next step: "Bu vaxt artıq tutulub. Başqa vaxt seçin." (Birbank).
- Empty: **"hələ … yoxdur"** for "no … yet" ("Bu kateqoriyada hələ sual yoxdur"), "Səbətiniz boşdur",
  "heç nə tapılmadı" for no results. All caught up: "Əla, bütün məlumatlar yenilənib 🎉" (Wolt).
- Success: "uğurla" + past passive ("Dəyişikliklər uğurla yadda saxlanıldı"); in sən voice "Sifarişin uğurla tamamlandı".
- Calques here: "hələ ki" and "Hal-hazırda sizin …" (Russian пока что / на данный момент у вас), "Konum" (Turkish for
  yer/məkan).

## Words to settle once
- Privacy = **Məxfilik**. "Gizlilik" is Turkish, "Konfidensiallıq" is a Russian calque.
- Settings: four words are in use (Ayarlar, Parametrlər, Nizamlamalar, Tənzimləmələr). Use one for your own product;
  when sending the user into the phone's own settings, use the label the phone shows (Android/Samsung: Parametrlər).
- A social **feed is not "lent"**. Of every source read, only TikTok writes "lent" ("Sizin üçün lent"); native products
  name the thing itself (paylaşımlar, videolar, ana səhifə) or what happens (sürüşdürmə).
- Platform feature names users already see (Android, YouTube UI): Ekran vaxtı, Narahat etməyin, Yuxu vaxtı rejimi,
  fasilə, Anladım, İndi yox, Vaxt bitdi. See `terms.jsonl`.

## Calque tells (see avoid.jsonl)
- Russian officialese: passive nominalisations ("Bildirişlərin aktiv edilməsi"), "Pul vəsaitləri … ödənilib",
  "sahib olmaq lazımdır" (нужно иметь), "Yüksək əlçatanlıq".
- English shapes: "Qarşılayın" for "Meet …", "sadə və sürətli şəkildə" for -ly adverbs, "Heç bir" + plural noun,
  "Dizayna görə təhlükəsizlik" for "secure by design".
- Turkish passing as az: "Bildirimler kapalı", "Molaya mı ihtiyacınız var?" seen in Firefox's az (not included in the
  data for licence reasons).
- Machine translation: Google Help and Airbnb help in az are labelled auto-translated; never copy their phrasing.
