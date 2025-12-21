**BU SAYFADA BELİRTİLMEYEN DİĞER DESTELER, AI VEYA ÜCRETLİ DEĞİŞİKLİKLER DAHİL, BENİMLE HİÇBİR BAĞLANTISI YOKTUR.**

# Kaishi 1.5k - Türkçe

Yeni başlayanlara temel Japonca kelimeleri öğretmek için tasarlanmış modern bir Anki kart destesi olan **Kaishi 1.5k**'nin genel erişim deposuna hoş geldiniz. Kaishi 1.5k oldukça modüler bir yapıya sahiptir ve bu sayfa, kart destesini istediğiniz gibi değiştirmek için kullanabileceğiniz çeşitli seçenekleri açıklamaya ayrılmıştır. Kart destesinin ön yüzü şöyle görünür:

<img src="https://github.com/donkuri/Kaishi/blob/main/pics/kaishi-front.png" alt="Front of a Card in Kaishi 1.5k" style="width: 100%; height: auto">
Gördüğünüz gibi, hem kelime hem de cümleler var, ancak kelime cümlede vurgulanmış, böylece önemli bilgileri hemen ayırt etmek kolaylaşıyor. Kelime iyi öğrenildikten sonra, kelime ilk sırada göründüğü için tekrar daha hızlı oluyor. İşte varsayılan destenin arka yüzü:

<img src="https://github.com/donkuri/Kaishi/blob/main/pics/kaishi-back.png" alt="Back of a Card in Kaishi 1.5k" style="width: 100%; height: auto">

Gördüğünüz gibi, hem kelime hem de cümleler var, ancak kelime cümlede vurgulanmış, böylece önemli bilgileri hemen ayırt etmek kolaylaşıyor. Kelimeye iyice aşina olunduğunda, kelime ilk başta göründüğü için tekrar daha hızlı oluyor. İşte varsayılan destenin arka yüzü:

[Japonca veya yoğunlaştırılmış öğrenme konusunda yeniyseniz, lütfen önce kılavuzu okuyun.](https://donkuri.github.io/learn-japanese/guide/)

### İçindekiler

- [Desteyi nereden edinebilirim?](#desteyi-nereden-edinebilirim)
- [Bu desteyi nasıl kullanırım?](#bu-desteyi-nasıl-kullanırım)
- [Diğer ilgili desteler](#diğer-ilgili-desteler)
- [Deste için hangi seçenekler mevcuttur?](#deste-için-hangi-seçenekler-mevcuttur)
- [Görüntüleri beğenmedim!](#görüntüleri-beğenmedim)
- [Bu kelimenin seslendirmesi hatalı!](#bu-kelimenin-seslendirmesi-hatalı)
- [Kaishi'yi başka bir deste üzerine nasıl içe aktarılır](#kaishiyi-başka-bir-deste-üzerine-nasıl-içe-aktarılır)
- [Destenin doğuşu](#destenin-doğuşu)
- [Deste çevirisi](#deste-çevirisi)
- [Bu deste bittikten sonra ne yapacağım?](#bu-deste-bittikten-sonra-ne-yapacağım)
- [Teşekkürler](#teşekkürler)

## Desteyi nereden edinebilirim?

Kart destesini, bu GitHub'ın [sürümler] (https://github.com/donkuri/Kaishi/releases/) sayfasından veya [AnkiWeb] (https://ankiweb.net/shared/info/1196762551) adresinden indirebilirsiniz. Kart destesinin inceleme aşamasında olmaması gerekir. **Kart destesi Anki 2.1.50+ sürümlerinde desteklenmektedir.**

## Bu desteyi nasıl kullanırım?]

Kaishi'nin genel olarak Japonca öğrenmeye nasıl uyum sağladığına dair bir açıklama için [kılavuza](https://donkuri.github.io/learn-japanese/guide/) bakın.

## Diğer ilgili desteler

ねむい, Kaishi 1.5k'yı temel alarak bir radikal kart destesi hazırladı ve bu destede bulunan her kanji radikalini, Kaishi'de bu radikalin bulunduğu ilk kelimeyle ilişkilendirdi. Ayrıca, Kaishi'de bulunmayan birkaç radikal daha da kapsıyor. **Kanji ile zorlanıyorsanız, bu kart destesini Kaishi ile paralel olarak kullanabilirsiniz**, çünkü kart destesi ilerledikçe kanji radikallerini tanıtarak, bunları daha verimli bir şekilde parçalara ayırmanıza yardımcı olur. Kart destesini [AnkiWeb'de burada](https://ankiweb.net/shared/info/1722008986) bulabilirsiniz. Teşekkürler ねむい!

## Deste için hangi seçenekler mevcuttur?

Kartlarınızı değiştirmek için kullanabileceğiniz birçok seçenek vardır. Kartları değiştirmek için Kaishi destesini seçin,`Gözat`ı tıklayın, desteden herhangi bir kart seçin ve sağ üstteki `Kartlar...`ı tıklayın.

### Ton Vurgusu

En önemli seçenek, kartlarınıza ton vurgusunu eklemek isteyip istemediğinizdir. Şu anda, ton vurgusunu öğrenmek gerekip gerekmediği konusunda topluluk içinde oldukça hararetli tartışmalar yaşanmaktadır. Biz orta yolcu bir yaklaşım benimsemeye karar verdik: ton vurgusu verileri sizin için hazır, kullanıp kullanmamak size kalmış. Kullanmamaya karar verirseniz, daha sonra istediğiniz zaman etkinleştirebilirsiniz. Ton vurgusunu etkinleştirmek çok kolaydır. İşte deste için `Arka Şablon` altındaki kart seçenekleri (`Arama` çubuğunun üzerindeki küçük noktaya tıklayın).

```CSS
<div lang="ja">
{{furigana:Word Furigana}}

<!-- This part enables pitch accent.

{{#Pitch Accent}}
	<br><div style='font-size: 24px'>{{Pitch Accent}}</div>
{{/Pitch Accent}} 

-->

<div style='font-size: 25px; padding-bottom:20px'>{{Word Meaning}}</div>
<div style='font-size: 25px;'>{{furigana:Sentence Furigana}}</div>
<div style='font-size: 25px; padding-bottom:10px'>{{Sentence Meaning}}</div>

{{Word Audio}}
{{Sentence Audio}}
<br>
{{Picture}}

{{#Notes}}
	<br>
	<div style="font-size: 20px; padding-top:12px">Note: {{Notes}}</div>
{{/Notes}}

<!-- This part enables pitch accent notes.

{{#Pitch Accent Notes}}
<div style="font-size: 20px; width: fit-content; max-width:40vw; margin: auto">
	<details><summary>Pitch Accent Notes</summary>
		<br>{{Pitch Accent Notes}}
	</details>
</div>
{{/Pitch Accent Notes}}

-->

</div>
```

Ton vurgusunu etkinleştirmek için, yorumları temsil eden tüm `<!--` ve `-->` kısımlarını şu şekilde çıkarmanız yeterlidir: 

```CSS
<div lang="ja">
{{furigana:Word Furigana}}

{{#Pitch Accent}}
	<br><div style='font-size: 24px'>{{Pitch Accent}}</div>
{{/Pitch Accent}} 

<div style='font-size: 25px; padding-bottom:20px'>{{Word Meaning}}</div>
<div style='font-size: 25px;'>{{furigana:Sentence Furigana}}</div>
<div style='font-size: 25px; padding-bottom:10px'>{{Sentence Meaning}}</div>

{{Word Audio}}
{{Sentence Audio}}
<br>
{{Picture}}

{{#Notes}}
	<br>
	<div style="font-size: 20px; padding-top:12px">Note: {{Notes}}</div>
{{/Notes}}

{{#Pitch Accent Notes}}
<div style="font-size: 20px; width: fit-content; max-width:40vw; margin: auto">
	<details><summary>Pitch Accent Notes</summary>
		<br>{{Pitch Accent Notes}}
	</details>
</div>
{{/Pitch Accent Notes}}

</div>
```

**Ton vurgu notasyonunun nasıl çalıştığını görmek için lütfen [bu konuya](https://github.com/donkuri/Kaishi/issues/104#issuecomment-3171889366) bakın.**

### Alt seçenekler

Değiştirebileceğiniz birkaç alt seçenek vardır.

#### Furigana
Furigana'yı çıkarmak istiyorsanız, arka şablondaki `furigana:` kısımlarını çıkarmanız yeterlidir.

#### Diğer kart seçenekleri

Görmek istediğiniz kartların türünü tamamen değiştirebilirsiniz. İşte Kaishi 1.5k'nın `Ön Şablonu`:

```CSS
<div lang="ja">
{{Word}}
<div style='font-size: 20px;'>{{Sentence}}</div>
</div>
```

Gördüğünüz gibi, sadece kelime ve cümle var. *Cümle* kartları istiyorsanız, `{{Word}}` kısmını çıkarın veya yerine `Sentence` yazıp geri kalanını çıkarın. *Kelime* kartları istiyorsanız, `<div style='font-size: 20px;'>{{Sentence}}</div>` kısmını çıkarmanız yeterlidir. Bunun yerine *ses* kartları istiyorsanız, her şeyi çıkarın ve `{{Word Audio}}`, `{{Sentence Audio}}` veya her ikisini de istiyorsanız ikisini birden ekleyin. 

#### Yazı tiplerini, yazı tipi boyutunu veya diğer stil seçeneklerini değiştirme

İşte Kaishi 1.5k'nin `Styling` şablonu:

```CSS
.card {
 font-family: "ヒラギノ角ゴ Pro W3", "Hiragino Kaku Gothic Pro", "Noto Sans JP", Osaka, "メイリオ", Meiryo, "ＭＳ Ｐゴシック", "MS PGothic", "MS UI Gothic", sans-serif;
 font-size: 44px;
 text-align: center;
}

img {
max-width: 300px;
max-height: 250px;
}

.mobile img {
max-width: 50vw;
}

/* This part defines the bold color. */
b{color: #5586cd}
```

Çeşitli stil seçeneklerini [burada](https://docs.ankiweb.net/templates/styling.html) bulabilirsiniz. Gördüğünüz gibi, Kaishi 1.5k stil sekmesinde doğrudan çok az seçenek kullanır. Farklı yazı tipleri elde etmek için `font-family` seçeneğini, yazı tipi boyutunu değiştirmek için `font-size` seçeneğini ve metnin hizalamasını değiştirmek için `text-align` seçeneğini değiştirebilirsiniz, örneğin metnin sola hizalanmasını istiyorsanız. Varsayılan olarak, Kaishi 1.5k kelimeleri **kalın** olarak renklendirir. Bunu değiştirmek için yukarıda gördüğünüz gibi `b{color: }` seçeneğini kullanabilirsiniz. O rengi elde etmek için hex kodu veya `red` gibi bir renk adı girmeniz yeterlidir. Renk istemiyorsanız, `b{color: }` kısmını tamamen çıkarmanız yeterlidir.

## Bu kelimenin seslendirmesi hatalı!

次 (つぎ) ve あげる gibi bazı kelimelerin seslerinin “yanlış” olduğu bildirilmiştir. Bunun nedeni, yeni başlayanların genellikle Japonca nazalizasyonu duymamaları (ve farkında olmamalarıdır); bu nazalizasyonda /g/ sesleri /n/ sesine daha yakın çıkabilir. Bunun nasıl çalıştığına dair açıklama için lütfen [bu videoyu](https://www.youtube.com/watch?v=xpzpbuFHVVU) izleyin. **Ne yazık ki, bu kelimelerin nazalize edilmemiş versiyonları şeklinde daha iyi sesler genellikle doğrudan mevcut değildir.**

## Kaishi'yi başka bir deste üzerine nasıl içe aktarılır

Core2k veya Tango N4-N5 (veya benzeri bir deste) kullanmaya başladıysanız ve Kaishi 1.5k'ya geçmek istiyorsanız, [Kuuube](https://github.com/Kuuuube) tarafından yazılan bu adımları takip edebilirsiniz.

1. Kaishi'yi .apkg dosyasıyla normal şekilde içe aktarın.
2. `Dosya > Dışa Aktar...` seçeneğine gidin ve Kaishi destesini `Düz Metin (.txt) Notları` kullanarak dışa aktarın. Diğer tüm ayarları varsayılan olarak bırakın.
3. Kaishi destesini silin.
4. Kaishi'yi içe aktarmak istediğiniz desteyi seçin, `Gözat`'ı seçin, herhangi bir kartı tıklayın, `ctrl + a` tuşlarına basın ve sol üst menüden `Notlar > Not Türünü Değiştir...`'i seçin. Seçtiğiniz tüm notların aynı not türüne ait olduğundan emin olun, aksi takdirde `Notlar > Not Türünü Değiştir...` seçeneği görünmeyebilir.
5. `Kaishi 1.5k` not türüne geçin. `Yeni` sütunundaki `Kelime` alanının, destenizin yanındaki kelime için kullandığı alanı gösterdiğinden emin olun.
  Mevcut destenizden Kaishi'de olmayan kartları silmek istemiyorsanız, diğer alanların da doğru yerlere hizalandığından emin olun. Aksi takdirde, varsayılanları kullanabilir ve `Kaydet`'i tıklayabilirsiniz.
6. 2. adımda dışa aktarılan Kaishi .txt dosyasını içe aktarın.
7. İçe aktarırken, Not Türü'nün `Kaishi 1.5k` olarak ve Destesi'nin içe aktarmak istediğiniz deste olarak ayarlandığından emin olun. 
  Kaishi'de olmayan kartları silmek istiyorsanız, `Tüm notları etiketle` seçeneğine `Kaishi` etiketini ekleyin.
8. “İçe Aktar”ı tıklayın.
9. Kaishi'de olmayan kartları silmek için destenizi seçin, “Gözat”ı tıklayın, sol menüden destenizi seçin, arama çubuğuna “-tag:Kaishi” ekleyin, herhangi bir kartı seçin, sol üst menüden “ctrl + a” tuşlarına basın ve “Notlar > Sil”e gidin.

**Core 2.3k üzerine içe aktarıyorsanız, lütfen [bunu](https://github.com/Manhhao/anki.transfer-review-history) inceleyin.**

## Görüntüleri beğenmedim!

Haklısın. Kart destesi için kullanmak üzere 1500 adet tutarlı ve ücretsiz resim bulmak çok zordu (bunun için tekrar teşekkürler [liarbeast](https://github.com/liarbeast)!). Sonuç olarak, bir dizi resim cümle veya kelimeyle tam olarak uyuşmuyor. Bu geçerli bir eleştiri ve resmi çıkarmak isterseniz, yapmanız gerekenler şunlar. `Tarayıcıda bir Kaishi kartına tıkladıktan sonra Cards...`'ı açın. `Back` şablonunu bulun. İçinde `{{Picture}}`'yi göreceksiniz. Bunu çıkarmanız yeterlidir. Alternatif olarak, her şeyi aşağıdakiyle değiştirin:

```html
<div lang="ja">
{{furigana:Word Furigana}}

<!-- This part enables pitch accent.

{{#Pitch Accent}}
	<br><div style='font-size: 24px'>{{Pitch Accent}}</div>
{{/Pitch Accent}} 

-->

<div style='font-size: 25px; padding-bottom:20px'>{{Word Meaning}}</div>
<div style='font-size: 25px;'>{{furigana:Sentence Furigana}}</div>
<div style='font-size: 25px; padding-bottom:10px'>{{Sentence Meaning}}</div>

{{Word Audio}}
{{Sentence Audio}}
<br>

{{#Notes}}
	<br>
	<div style="font-size: 20px; padding-top:12px">Note: {{Notes}}</div>
{{/Notes}}

<!-- This part enables pitch accent notes.

{{#Pitch Accent Notes}}
<div style="font-size: 20px; width: fit-content; max-width:40vw; margin: auto">
	<details><summary>Pitch Accent Notes</summary>
		<br>{{Pitch Accent Notes}}
	</details>
</div>
{{/Pitch Accent Notes}}

-->

</div>
```

## Destenin doğuşu

Bu deste, Tyogin ve benim [TMW discord sunucusunda](https://learnjapanese.moe/join/) yaptığımız bir tartışmadan doğmuştur. İkimiz de o dönemde popüler olan başlangıç seviyesi destelerin can sıkıcı kusurları olduğunu hayıflanıyorduk. Yeni başlayanlar, çeşitli sorunlar nedeniyle Core 2k ve Tango'yu kullanırken sürekli kafaları karışıyordu. Tango'da, Tayland balık sosu olan ナンプラー gibi bazı anlaşılması zor kelimeler vardı ve birçok kişi, destenin büyük bir bölümünü kaplayan temel ifadeler ve ülke isimleriyle pek ilgilenmiyordu. Destenin alanları çok kötü biçimlendirilmişti, bu da desteyi asıl amaçlanan şekilde, yani cümle kartları olarak kullanmayı imkansız hale getiriyordu. Core 2k ise modülerdi, ancak birçok yanlış çeviri, eksik veya alakasız resimler içeriyordu ve bazı cümleler pek kullanışlı değildi, hatta bazen kullanılan kelimenin anlamını yansıtmıyordu.

Bu iki sorun da o kadar can sıkıcıydı ki, her iki haftada bir yeni başlayanlar bu konuda sorular soruyordu. Tyogin, sorunu kendimiz çözmemizi önerdi ve bu sorunları gidermek için küçük bir ekip oluşturuldu. Çoğunlukla Core2k, Core10k, Tango N4 ve Tango N5'ten veri aldık. Ardından verileri birleştirdik, çeşitli Yomichan/Yomitan sıklık sözlüklerini kullanarak kelimeleri sıklıklarına göre sıraladık ve yaklaşık 1500 kelime seçtik. Daha sonra her kelimenin çevirisini düzelttik, her kelime için en uygun cümleyi seçtik ve gerekirse cümleyi düzelttik. Seçtiğimiz 1500 cümleden yaklaşık 120 cümleyi düzeltmek zorunda kaldık. Ardından, [AJT Japanese](https://ankiweb.net/shared/info/1344485230) sitesinden uygun ses kaydı bulunmayan kelimeler için hem ses tonu verilerini hem de kelime ses kayıtlarını elde ettik ve iki kişilik bir ekip (Karifurai ve cindsa) ses tonu verilerini doğruladı. Ayrıca, gerekli olan kelimeler için ton vurgu notları da eklediler. Ardından, ses kaydındaki sessiz kısımları kırptık ve çeşitli dosyalar arasındaki ses seviyesini normalleştirdik. Bunun üzerine, kelimeler ve cümleler için AJT Japanese'den furigana da ürettik. Bundan sonra, desteğin varsayılan sürümünde kullanılacak temel ipucu hedefli cümle kartı CSS'sini tasarladık. Son olarak, mümkün olduğunca az hata olması için desteği birden fazla kişi düzeltti.

Kaishi, 開始 yazılır ve “başlangıç, başlangıç” anlamına gelir. Bunun uygun olduğunu düşündük ve bu ismi seçtik. Umarız bu deste, Japonca öğrenme yolculuğunuz için harika bir başlangıç olur.

## Bu deste bittikten sonra ne yapacağım?

Henüz başlamadıysanız [madenciliğe başlayın](https://donkuri.github.io/learn-japanese/guide/#consuming-native-content). Madencilik not türlerinin listesi için [buraya](https://github.com/donkuri/japanese-resources/?tab=readme-ov-file#mining) bakın.

## Deste çevirisi

Deck'i ana dilinize çevirmekle ilgileniyorsanız, lütfen [GitHub tracker](https://github.com/donkuri/Kaishi/issues) üzerinde bir konu açın. Sunum **[Rusça](https://github.com/NeonGooRoo/KaishiRu)**, **[Endonezce](https://ankiweb.net/shared/info/1512066033)**, **[Vietnamca](https://github.com/duy103zxc/kaishi-vi/releases)**, **[Ukraynaca](https://github.com/maksiksq/KaishiUa)**, **[Brezilya Portekizcesi](https://github.com/nonsolvent/Kaishi-pt-BR)**, **[İspanyolca](https://github.com/Dogi5/Kaishi-ESP)**, **[Mandarin](https://github.com/maimemo/kaishi-zh-cn/)** ve **[Fransızca](https://github.com/khmskhmskhms/kaishi-FR)**.

## Teşekkürler

Bu deste şu kişilerin yardımıyla oluşturulmuştur:

[栗](https://github.com/donkuri/) - ana mimar, tüm teknik konular, çeviriler, düzeltmeler

Tyogin - ana mimar, ilk 200 kartı yeniden sıraladı, cümleleri değiştirdi, düzeltmeler yaptı

shoui - tüm desteyi düzeltti, çevirileri düzeltti

Julian - not eklemeye yardım etti ve bazı cümle çevirilerini kontrol etti

karifurai - ilk 750 kartın ton vurgusunu doğruladı ve ton notları ekledi

cindsa - son 750 kartın ton vurgusunu doğruladı ve ton notları ekledi

[Kuuube](https://github.com/Kuuuube) - FFmpeg kullanımını önerdi, yukarıdaki Kaishi 1.5k bölümüne kartların aktarılmasını yazdı

[stephenmk](https://github.com/stephenmk) - Kaishi 1.5k üzerinde Jmdict Furigana aracını çalıştırarak furigana'yı düzeltti, bkz. v1.3.0

[Kaanium](https://github.com/kaanium) - desteyi yazma sürümüne dönüştürmek için bir komut dosyası oluşturulmasına yardımcı oldu

[Lars](https://github.com/liarbeast) - [irasutoya](https://www.irasutoya.com/) sitesinden resimler ekledi

Bu araçlar desteğin oluşturulmasında kullanıldı:

[AJT Japanese](https://github.com/Ajatt-Tools/Japanese) - ton vurgusu, furigana ve bazı sesler bu eklenti kullanılarak oluşturuldu

[FFmpeg](https://ffmpeg.org/) - çeşitli ses dosyalarındaki bazı sessiz kısımları çıkarmak için kullanıldı

[Tenacity](https://tenacityaudio.org/) - çeşitli ses dosyalarındaki kesme seslerini düzenlemek için kullanıldı.

Ayrıca, TMW discord sunucusunun birçok üyesinden, desteğin adı da dahil olmak üzere çeşitli fikirler aldık. Cümleler ise Ankiweb'de bulunan çeşitli Core destelerinden alınmıştır.




