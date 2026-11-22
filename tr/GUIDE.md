# Turkish product copy: how native products write it

Distilled from `phrasebook.jsonl` (native sources), `terms.jsonl` (platform UI names) and `avoid.jsonl` (calques).
Round 2, November 2026: Instagram web (tr_TR bundle, ~2.7k strings paired with en_US), TikTok web (2.5k keys), Duolingo
(3.8k keys), YouTube ytcfg tables, Android AOSP `values-tr`, Apple's iPhone guide, Spotify, Netflix, Storytel, Facebook.
Big Turkish consumer sites (Getir, Trendyol, Yemeksepeti, Hepsiburada, sahibinden) refuse automated fetches, so the
Turkish-first voice comes mostly from Storytel, fizy, BiP, Paycell and the banks. A native speaker has the last word on
every rule.

## Register
- Friendly consumer apps speak **sen** with a bare imperative: Instagram ("Günlük sınırına ulaştın", "Tekrar dene"),
  Duolingo ("Süren doldu!", "istediğin zaman iptal et"), Spotify ("İstediğin zaman iptal et"), Facebook login ("Şifreni
  mi unuttun?"), Storytel, fizy, Paycell, TOD.
- Platform utilities speak **siz**: YouTube ("Bağlantınızı kontrol edin"), TikTok ("Ekran başında kesintisiz {num}
  dakika geçirdiniz"), Android, Apple, Netflix, WhatsApp, Pinterest; banks and carriers too (Enpara, Garanti, Turkcell).
  Their *buttons* are still bare imperatives ("Abone ol", "Tekrar dene", "Giriş yap").
- An app that sits on top of Instagram and YouTube and talks about the user's habits is closest to Instagram: sen.
- Pick one per surface and keep it. Real slips: Storytel "Şimdi … ödeyin … iptal edebilirsin" in one sentence,
  fizy "sahip olduğun … üzerinizdeki", Duolingo's billing bundle in siz inside a sen app, Instagram's ad panel ("Bu
  reklamı neden görüyorsunuz?") in siz.
- "Your" lives in the suffix: "çalma listelerin", "Günlük sınırına", "şifreni", never "senin" unless stressed ("Ne
  çalacağına yalnızca sen karar ver", Spotify).

## Buttons and short labels
- Bare verb, sentence case: Tekrar dene, Devam et, Kapat, Kaydet, Sil, Paylaş, Atla, Bitti, Anladım, Şimdi değil,
  İptal (Android, TikTok, YouTube, Instagram). Meta and Duolingo write Title Case ("Takip Et", "Facebook ile Giriş Yap",
  "Şimdi Değil"); TikTok, YouTube and Android keep sentence case. Choose one for your product.
- Log in: **Giriş yap** (Meta, Duolingo, TikTok) or **Oturum aç** (YouTube, Google, Duolingo). Log out: Çıkış yap.
  Sign up: Kaydol.
- Open the app: "Uygulamayı aç" (Instagram, YouTube), "Instagram'ı aç", "TikTok'u aç". Get the app: "Uygulamayı indir"
  (TikTok), "Instagram uygulamasını indir". Never "Uygulamayı edinin" (Pinterest) or "Premium'u edin" (Spotify).
- Dialog questions take **-sın mı?**: "İndirilen tüm içerikler silinsin mi?" (YouTube), "Arka plan etkinliği
  sınırlansın mı?" (Android), "Bugün uyku saatleriniz kapatılsın mı?" (TikTok). Don't put an accusative object in
  front of it ("Otomatik oynatmayı kapatılsın mı?" is a YouTube bug).
- Native lines drop "Lütfen" and "-maktadır": "Bir şeyler ters gitti", not "Teknik bir sorun yaşanmaktadır. Lütfen
  daha sonra tekrar deneyiniz."
- Capitals: Turkish İ/I. "ABONE OL", "ABONELİKTEN ÇIK" (YouTube), "ÜCRETSİZ HAFTAMI BAŞLAT" (Duolingo). Uppercase
  with the tr locale only.
- Abbreviations after numbers: "dk", "sa", "sn", with or without a dot ("{n} dk. kaldı", YouTube; "Ertele (10 dk)",
  TikTok). Instagram spells out "saat", "dakika".

## Grammar traps
- **No variable before a case suffix.** The suffix depends on the word: "{username}'(n)in", "@{username}'i takibi
  bırak?" ship broken in Instagram. Build the sentence so the name stands alone: "{site} için", "{name} ile",
  "Gönderi: {name}", "{site} yine de açılsın mı?". A fixed name may take its suffix with an apostrophe:
  "Instagram'ı", "YouTube'u", "TikTok'u", "Facebook'u".
- **Nouns stay singular after a number**: "5 dakika", "31 önerilen gönderi", "{count} video". Plural forms are
  usually one string.
- Apostrophes only before suffixes on proper names ("Ekran Süresi'ne", Apple); "bilgisayarlar'da" (Instagram Help)
  is wrong.
- Never build a sentence from fragments glued in English order ("Kendini {Express}", "{joy} saç", Instagram).
- A UI name inside a sentence goes in quotes and the suffix moves to a helper noun: "“Abonelikler” sayfasında aç",
  "“Ekle” seçeneğine dokun".

## Stock phrases natives reach for
| English idea | Native tr | Source |
|---|---|---|
| cancel anytime | İstediğin zaman iptal et | Spotify, Duolingo |
| you keep your stuff | … sende kalır | Spotify |
| X days free | {n} gün ücretsiz, İlk 3 ay boyunca ücretsiz | Storytel, Spotify |
| start my free trial | Ücretsiz denememi başlat, ÜCRETSİZ HAFTAMI BAŞLAT | Duolingo |
| one-time payment | tek seferlik bir ödeme | Duolingo |
| recurring billing | Ödemeler yenilenir / Yinelenen faturalandırma | Duolingo / YouTube |
| we'll remind you before the trial ends | Deneme süreniz sona ermeden 7 gün önce size hatırlatma yapacağız. | YouTube |
| enjoy it, uninterrupted | tadını kesintisiz çıkar | Spotify, fizy |
| anytime, anywhere | İstediğin zaman, istediğin yerde | Storytel, fizy |
| don't miss out | Yenilikleri kaçırma | Storytel |
| save it for later | Sonrası için kaydet | Instagram |
| you're all caught up | Hepsini gördün | Instagram |
| you can change this in Settings | Bunu istediğin zaman Ayarlardan değiştirebilirsin. | Instagram |
| watch ad-free | Videoları reklamsız izleyin | YouTube |
| we never share your data | Verileriniz şifrelidir ve kimseyle paylaşılmaz. | BiP |

## Limits, time, quiet hours
- Limit reached: **"Günlük sınırına ulaştın"**, "Instagram'ı kapatma zamanı geldi. Yarın tekrar kullanabilirsin.",
  "Bugün Instagram'ı 5 dakika daha kullanabilirsin." (Instagram). Meta mixes "süre sınırı" and "zaman sınırı"; pick
  "süre sınırı" or plain "sınır".
- Time's up: **"Süre doldu"** (YouTube sleep timer), **"Süren doldu!"** (Duolingo). "Süre dolmak" is the verb pair in
  all four products; "Süreniz dolduğunda uygulama kapanır" (Google).
- Nudges: "Mola verme zamanı geldi mi?", "TikTok'u kapatmaya hazır mısınız?" (TikTok); "Yavaşlamaya hazır mısın?",
  "Şimdi uygulamayı kapatmak için iyi bir zaman." (Instagram).
- A time inside a sentence: "{time} saatine kadar" (Instagram), or after a colon: "Şu saatten sonra kullanmaya devam
  edebilirsin: {time}." (Instagram).
- Night: Instagram "Uyku modu" ("Uyku modundasın"), TikTok "Uyku saatleri", Android "Uyku Vakti modu", "Uyku vakti";
  Do Not Disturb "Rahatsız Etmeyin" (Android) / "Rahatsız Etme" (Apple); Focus "Odak" (Apple).
- Screen time: "Ekran süresi" (Digital Wellbeing, TikTok), "Ekran Süresi" (Apple), "Günlük ekran süresi" (TikTok),
  "Süre İzinleri" (Apple's Time Allowances), "Uygulama zamanlayıcıları" (Android).
- Snooze is "Ertele (10 dk)" (TikTok; its "Gecikme" is a bug). More time: "Süre ekle" (YouTube), "Daha fazla zaman
  iste" (Instagram).

## Errors, empty screens, offline
- Base error: **"Bir şeyler ters gitti"** (TikTok, Storytel), "Bir sorun oluştu" (Instagram), "Bir hata oluştu"
  (YouTube, Duolingo). Cheerful: "Hay aksi, bir sorun oluştu" (Instagram).
- Always the next step: "Biraz sonra tekrar dene", "İnternete bağlanıp tekrar deneyin" (TikTok), "Bağlantınızı kontrol
  edip tekrar deneyin" (YouTube). A failure we own: "Instagram'a bağlanamadık." (Instagram).
- Short failed states take the -(y)AmAdI passive: "Yüklenemedi.", "İndirilemedi", "Yorum paylaşılamadı.", "Giriş
  yapılamadı. Tekrar dene." (Instagram, YouTube).
- Offline = **çevrimdışı**: "İnternete bağlı değilsiniz", "İnternet bağlantısı yok", "İnternet bağlantısı
  bekleniyor...", "Video çevrimdışıyken kullanılamıyor" (YouTube); "İnternet bağlantını kaybettin!" (Duolingo).
- Empty: **"Henüz … yok"** ("Henüz video yok", TikTok; "Henüz hiç takipçin yok", Duolingo), bare "… yok" for lists
  ("Son arama yok.", Instagram; "Bildirim yok", Android; "İndirilen video yok", YouTube). Say where things will appear:
  "İndirdiğiniz videolar burada gösterilir" (YouTube).
- Storage: "Depolama alanı dolu" (YouTube), "Depolama alanı bitiyor" (Android), "Yer aç" (Android).
- Purchases: "Satın alım onaylandı!", "Satın alım başarısız oldu!" (Duolingo).

## Words to settle once
- Feed = **akış** (Instagram "akışta daha yukarıda", Facebook "Akış", YouTube "Ana Sayfa özet akışınıza"). Unlike
  Azerbaijani, the word is native here. Facebook help still has the older "Haber Kaynağı".
- Reels is never translated; one video is "Reels videosu", plural "Reels videoları" (Instagram, Facebook). Shorts stays
  Shorts (YouTube). TikTok's For You is **"Sizin İçin"**: a siz form, but it is a name, so quote it as is.
- Following: Instagram's feed choice is **"Takip ettiklerin"**, its profile button state "Takiptesin". TikTok's nav key
  is "Takipte", its button state "Takip ediliyor", and its feed is "Takip edilenler" in running text.
- Subscriptions (YouTube): **"Abonelikler"** (page title); Subscribe "Abone ol". Watch later: **"Daha sonra izle"**
  ("Daha sonra izle'ye kaydet"). Downloads: **"İndirilenler"** (YouTube, Android).
- Suggested: "Senin için önerilenler" (Instagram), "Önerilenler" (Instagram Explore); People You May Know "Tanıyor
  Olabileceğin Kişiler" (Facebook). Sponsored "Sponsorlu", Ad "Reklam" (Facebook, Instagram, YouTube).
- Picture in picture: **"Pencere içinde pencere"** (Android, YouTube) but **"Resim İçinde Resim"** on iOS (Apple).
  Background play "Arka planda oynatma", sleep timer "Uyku modu zamanlayıcı" (YouTube).
- Restore purchases: only **"Geri yükle"** is on public pages (Android, YouTube); "Satın alımları geri yükle" lives in
  store dialogs that were not reachable.
- Privacy = Gizlilik, Terms = Koşullar (Duolingo has four names for Terms; pick one), Settings = Ayarlar.
- Free = **ücretsiz** (Spotify, Duolingo, YouTube, Storytel, Pinterest, WhatsApp).

## Calque tells (see avoid.jsonl)
- "edin/edinin" for get (Pinterest, Spotify): say indir, al, ol ("Premium üyesi olun", YouTube).
- Passive nominal titles: "Instagram'da günlük süre sınırının ayarlanması", "Ekran Süresi'ni kapatma" are the
  help-centre voice (Meta, Apple), never UI titles.
- "Konsantrasyon modu" for Focus (Apple: Odak); "anında ilet bildirimi" for push (TikTok: "Anlık bildirimler");
  "Kablosuz" for Wi-Fi (Android); "Giriş yapılı olmadığı için" (Storytel).
- Billing-department Turkish: "ücret tahsil edilmeyecektir" (Netflix), "-bulunmaktadır" (Storytel).
- Meaning drift, checked against the English: Instagram "log in" became "kaydol"; YouTube "Not available" became
  "Sonuç bulunamadı"; TikTok "Delay" became "Gecikme".
- On Turkish-first sites (BiP, ininal, Garanti) the English is the translated side; don't take it as the source of
  meaning.
- Google's and YouTube's Turkish help pages are labelled AI-translated: take their feature names, not their phrasing.
