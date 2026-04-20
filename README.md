**BU SAYFADA BELIRTİLMEYEN DİĞER TÜM KART DESTELERİ, YAPAY ZEKA VEYA ÜCRETLİ DEĞİŞİKLİKLER DAHİL OLMAK ÜZERE, BENİMLE HERHANGİ BİR BAĞLANTISI BULUNMAMAKTADIR.**

# Kaishi 1.5k

Yeni başlayanlara temel Japonca kelime dağarcığını öğretmek için hazırlanmış modern bir Anki destesi olan **Kaishi 1.5k**’nin genel erişime açık depo sayfasına hoş geldiniz. Kaishi 1.5k son derece modüler bir yapıya sahiptir ve bu sayfa, desteyi kendi tercihlerinize göre özelleştirmek için kullanabileceğiniz çeşitli seçenekleri açıklamaya ayrılmıştır. Destenin ön yüzü şu şekilde görünmektedir:

<img src="https://github.com/donkuri/Kaishi/blob/main/pics/kaishi-front.png" alt="Kaishi 1,5k kartının ön yüzü" style="width: 100%; height: auto">

Gördüğünüz gibi, hem kelime hem de cümleler mevcut; ancak kelime cümle içinde vurgulanmış durumda, bu da önemli bilgiyi hemen ayırt etmeyi kolaylaştırıyor. Kelime iyice öğrenildikten sonra, kelime ilk sırada yer aldığı için tekrar yapmak daha hızlı oluyor. İşte varsayılan kart destesinin arka yüzü:

<img src="https://github.com/donkuri/Kaishi/blob/main/pics/kaishi-back.png" alt="Kaishi 1,5k kartının arka yüzü" style="width: 100%; height: auto">

Diğer çoğu Core tipi destenin aksine, burada furigana kelimenin okunuşunu gösterir ve anlamı hemen altında yer alır. Ardından kelimenin ve cümlenin ses kaydı dinleyebilirsiniz. İsterseniz, tonlama da ekleyebilirsiniz; bunun için aşağıya bakın. O kartla ilgili notlar varsa, bunlar aşağıda görüntülenir.

[Japonca öğrenmeye yeni başladıysanız veya dil öğrenme programına yeni katıldıysanız, lütfen önce kılavuzu okuyun.](https://donkuri.github.io/learn-japanese/guide/)

### İçindekiler

- [Desteyi nereden bulabilirim?](#where-do-i-get-the-deck)
- [Bu deste nasıl kullanılır?](#how-do-i-use-this-deck)
- [Diğer ilgili desteler](#other-related-decks)
- [Deste için hangi seçeneler mevcut?](#what-options-are-available-for-the-deck)
- [Bu resimleri beğenmedim!](#i-dont-like-the-images)
- [Cümlelerin sürekli açık kalmasından memnun değilim!](#i-dont-like-having-sentences-always-on)
- [Bu kelimenin ses kaydı yanlış!](#the-audio-for-this-word-is-wrong)
- [Kaishi destesini başka bir destenin üzerine nasıl ekleyebilirim?](#how-to-import-kaishi-on-top-of-another-deck)
- [Destenin doğuşu](#the-genesis-of-the-deck)
- [Kart destesinin çevirisi](#translation-of-the-deck)
- [Bu deste bittikten sonra ne yapmalıyım?](#what-do-i-do-after-this-deck)
- [Katkıda Bulunanlar](#credits)

## Desteyi nereden bulabilirim?

You can either get the deck on the [releases](https://github.com/donkuri/Kaishi/releases/) page of this GitHub or on [AnkiWeb](https://ankiweb.net/shared/info/1196762551), provided the deck is not undergoing review. **The deck is supported on Anki 2.1.50+.**

## Bu deste nasıl kullanılır?

Kaishi'nin genel olarak Japonca öğrenme sürecine nasıl uyum sağladığına dair bir açıklama için [kılavuza] bakın(https://donkuri.github.io/learn-japanese/guide/).

## Diğer ilgili desteler

ねむい, Kaishi 1.5k'yı temel alarak bir kök kart destesi hazırladı; bu destede yer alan her kanji kökünü, Kaishi'de o kökün bulunduğu ilk kelimeyle eşleştirdi. Ayrıca, Kaishi'nin ana içeriğinde bulunmayan birkaç kök daha da kapsıyor. **Kanji öğrenirken zorlanıyorsanız bu desteyi Kaishi ile birlikte kullanabilirsiniz**, çünkü ilerledikçe kanji köklerini tanıtarak bunları daha verimli bir şekilde ayrıştırmanıza yardımcı oluyor. Bu desteyi [AnkiWeb'de burada](https://ankiweb.net/shared/info/1722008986) bulabilirsiniz. Teşekkürler ねむい!

## Deste için hangi seçeneler mevcut?

Kartlarınızı değiştirmek için kullanabileceğiniz çeşitli seçenekler mevcuttur. Kartları değiştirmek için Kaishi destesini seçin, `Gözat` düğmesine tıklayın, desteden herhangi bir kartı seçin ve sağ üst köşedeki `Kartlar...` düğmesine tıklayın.

### Tonlama

En önemli seçenek, kartlarınıza tonlama aksanını dahil etmek isteyip istemediğinizdir. Şu anda, tonlama aksanını öğrenip öğrenmeme konusu topluluk içinde oldukça hararetli tartışmalara yol açmaktadır. Biz orta yolu seçtik: tonlama aksanı verileri hazırdır, kullanmak isteyip istemediğinize siz karar verirsiniz. Kullanmamaya karar verirseniz, daha sonra istediğiniz zaman etkinleştirebilirsiniz. Tonlama aksanını etkinleştirme işlemi oldukça basittir. İşte destenin `Arka Şablonu` altındaki kart seçenekleri (`Arama` çubuğunun üzerindeki küçük noktaya tıklayın.)

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

Tonlama aksanını etkinleştirmek için, aşağıdaki gibi yorumları temsil eden tüm `<!--` ve `-->` kısımlarını kaldırmanız yeterlidir: 

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

**Tonlama aksanı notasyonunun nasıl işlediğini görmek için lütfen [bu konuya](https://github.com/donkuri/Kaishi/issues/104#issuecomment-3171889366) bakın.**

### İkincil seçenekler

Değiştirebileceğiniz birkaç küçük ayar var.

#### Furigana
Furigana'yı kaldırmak isterseniz, arka şablondaki `furigana:` kısımlarını silmeniz yeterlidir.

#### Diğer kart seçenekleri

Görmek istediğiniz kart türünü tamamen değiştirebilirsiniz. İşte Kaishi 1.5k'nın `Ön Şablonu`:

```CSS
<div lang="ja">
{{Word}}
<div style='font-size: 20px;'>{{Sentence}}</div>
</div>
```

Gördüğünüz gibi, elimizde sadece kelime ve cümle var. *Cümle* kartları istiyorsanız, `{{Word}}` kısmını kaldırmanız ya da yerine `Sentence` yazıp geri kalanını silmeniz yeterlidir. *Kelime* kartları istiyorsanız, `<div style=‘font-size: 20px;’>{{Sentence}}</div>` kısmını çıkarın. Bunun yerine *ses* kartları istiyorsanız, her şeyi çıkarın ve `{{Word Audio}}`, `{{Sentence Audio}}` veya her ikisini de istiyorsanız ikisini birden ekleyin.

#### Yazı tiplerini, yazı tipi boyutunu veya diğer stil seçeneklerini değiştirme

İşte Kaishi 1.5k’nın `Stil Oluşturma` şablonu:

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

Çeşitli stil seçeneklerini [burada](https://docs.ankiweb.net/templates/styling.html) bulabilirsiniz. Gördüğünüz gibi, Kaishi 1.5k stil sekmesinde doğrudan çok az seçenek kullanıyor. Farklı yazı tiplerini elde etmek için `font-family` seçeneğini, yazı tipi boyutunu değiştirmek için `font-size` seçeneğini ve metnin hizalamasını değiştirmek için `text-align` seçeneğini değiştirebilirsiniz; örneğin, metnin sola hizalanmasını istiyorsanız. Varsayılan olarak, Kaishi 1.5k **kalın** yazılan kelimeleri renklendirir. Bunu değiştirmek için yukarıda görebileceğiniz gibi `b{color: }` seçeneğini kullanabilirsiniz. Bunun yerine o rengi elde etmek için bir onaltılık kod veya `red` gibi bir renk adı girmeniz yeterlidir. Renk istemiyorsanız, `b{color: }` kısmının tamamını kaldırmanız yeterlidir.

## Cümlelerin sürekli açık kalmasından memnun değilim!

Bazı kişiler cümleyi her zaman önlerinde görmek istemeyebilir. Bu tamamen makul bir durumdur, zira bazı kişiler sonunda sadece cümleleri ezberlemiş olurlar. Buradaki amaç, size bağlam sunmaktır; çünkü anlam her zaman bağlam içinde bulunur. İsterseniz, [bu konudaki yorumu](https://github.com/donkuri/kaishi/issues/131#issuecomment-3968847411) takip ederek ön ve stil şablonunuzu değiştirip bunları bulanıklaştırabilirsiniz. Bu fikir için [Hit2Skill](https://github.com/Hit2Skill) 'e teşekkür ederiz!

## Bu kelimenin ses kaydı yanlış!

次 (tsugi) ve あげる gibi bazı kelimelerin ses kayıtlarının “yanlış” olduğu bildirildi. Bunun nedeni, yeni başlayanların genellikle Japonca'daki nazalizasyonu duymamaları (ve bunun farkında olmamaları)dır; bu durumda /g/ sesleri /n/ sesine daha yakın çıkabilir. Bunun nasıl işlediğine dair açıklama için lütfen [bu videoyu](https://www.youtube.com/watch?v=xpzpbuFHVVU) izleyin. **Ne yazık ki, bu kelimelerin nazal olmayan versiyonları şeklinde daha iyi ses kayıtları genellikle doğrudan bulunmamaktadır.**

## Kaishi destesini başka bir destenin üzerine nasıl ekleyebilirim?

Eğer Core2k veya Tango N4-N5 (ya da benzeri bir deste) ile başlamışsanız ve Kaishi 1.5k'ya geçmek istiyorsanız, [Kuuube](https://github.com/Kuuuube) tarafından yazılan bu adımları takip edebilirsiniz.

1. Kaishi'yi .apkg dosyasıyla normal şekilde yükleyin.
2. `Dosya > Dışa Aktar...` seçeneğine gidin ve Kaishi destesini `Düz Metin Notları (.txt)` seçeneğini kullanarak dışa aktarın. Diğer tüm ayarları varsayılan olarak bırakın.
3. Kaishi destesini silin.
4. Kaishi'yi içe aktarmak istediğiniz desteyi seçin, `Gözat`'ı seçin, herhangi bir kartı tıklayın, `ctrl + a` tuşlarına basın ve sol üst menüden `Notlar > Not Türünü Değiştir...`'i seçin. Seçtiğiniz tüm notların aynı not türünde olduğundan emin olun, aksi takdirde `Notlar > Not Türünü Değiştir...` görünmeyebilir.
5. Not türünü `Kaishi 1.5k` olarak değiştirin. `Yeni` sütunundaki `Kelime` alanının, yanındaki kelime için destenizin kullandığı alanı gösterdiğinden emin olun.
    Mevcut destenizden Kaishi'de olmayan kartları silmeyi düşünmüyorsanız, diğer alanlarınızın da doğru yerlere hizalandığından emin olun. Aksi takdirde varsayılanları kullanabilir ve `Kaydet`'i tıklayabilirsiniz.
6. 2. adımda dışa aktarılan Kaishi .txt dosyasını içe aktarın.
7. İçe aktarma sırasında, Not Türü'nün `Kaishi 1.5k` olarak ayarlandığından ve Destek'in üzerine içe aktarmak istediğiniz desteye ayarlandığından emin olun. 
  Kaishi'de olmayan kartları silmeyi planlıyorsanız, `Tüm notları etiketle` seçeneğine `Kaishi` etiketini ekleyin.
8. `İçe Aktar`'a tıklayın.
9. Kaishi'de olmayan kartları silmek için destenizi seçin, `Gözat`'a tıklayın, sol menüden destenizi seçin, arama çubuğuna ` -tag:Kaishi` ekleyin, herhangi bir kartı seçin, `ctrl + a` tuşlarına basın, sol üst menüden `Notlar > Sil`'e gidin.

**Core 2.3k sürümünün üzerine aktarım yapıyorsanız, lütfen [buraya] bakın(https://github.com/Manhhao/anki.transfer-review-history).**

## Bu resimleri sevmiyorum!

Haklısın. Kart destesi için kullanılacak 1500 adet tutarlı ve telifsiz resim bulmak gerçekten çok zordu (bunun için [liarbeast](https://github.com/liarbeast)‘e tekrar teşekkürler!). Sonuç olarak, bazı resimler cümle veya kelimeyle tam olarak uyuşmuyor. Bu geçerli bir eleştiri ve eğer resmi çıkarmak isterseniz, yapmanız gerekenler şunlar: Tarayıcıda bir Kaishi kartına tıkladıktan sonra `Kartlar.`'ı açın. `Geri` şablonunu bulun. İçinde `{{Picture}}`'yi göreceksiniz. Onu çıkarın. Alternatif olarak, her şeyi aşağıdakiyle değiştirin:

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

Bu deste, [TMW Discord sunucusunda](https://learnjapanese.moe/join/) Tyogin ile aramızda geçen bir sohbetten doğdu. İkimiz de o dönemde popüler olan başlangıç destelerinin can sıkıcı kusurları olduğunu hayıflanıyorduk. Yeni başlayanlar, çeşitli sorunlar nedeniyle Core 2k ve Tango'yu kullanırken sürekli kafaları karışıyordu. Tango'da, Tayland balık sosu olan ナンプラー gibi anlaşılması zor kelimeler vardı ve birçok kişi, destenin büyük bir bölümünü kaplayan temel ifadeler ve ülke isimleriyle pek ilgilenmiyordu. Destenin alanları çok kötü biçimlendirilmişti, bu da desteyi asıl amaçlanan şekilde, yani cümle kartları olarak kullanmaktan başka bir şekilde kullanmayı imkansız hale getiriyordu. Öte yandan Core 2k modülerdi, ancak çok sayıda yanlış çeviri, eksik veya alakasız resimler içeriyordu ve bazı cümleler pek kullanışlı değildi, hatta bazen kullanılan kelimenin anlamını bile yansıtmıyordu.

Bu iki sorun da o kadar can sıkıcıydı ki, her iki haftada bir yeni başlayanlar bu konularla ilgili sorular soruyordu. Tyogin, sorunu kendimiz çözmemizi önerdi ve bu sorunları gidermek üzere küçük bir ekip oluşturuldu. Verilerimizi çoğunlukla Core2k, Core10k, Tango N4 ve Tango N5 kaynaklarından aldık. Ardından verileri birleştirdik, çeşitli Yomichan/Yomitan sıklık sözlüklerini kullanarak kelimeleri sıklığa göre sıraladık ve yaklaşık 1500 kelime seçtik. Ardından her kelimenin çevirisini düzelttik, her kelime için en uygun cümleyi seçtik ve gerekirse cümleyi düzelttik. Seçtiğimiz 1500 cümleden yaklaşık 120'sini düzeltmemiz gerekti. Bunun ardından, [AJT Japanese](https://ankiweb.net/shared/info/1344485230) kaynaklarından uygun ses kaydı bulunmayan kelimeler için hem tonlama aksanı verilerini hem de kelime seslerini elde ettik ve iki kişilik bir ekip (Karifurai ve cindsa) tonlama aksanı verilerini doğruladı. Ayrıca, gerekli olan kelimeler için tonlama aksanı notları eklediler. Daha sonra ses dosyalarındaki sessiz kısımları kırptık ve çeşitli dosyalar arasındaki ses seviyesini normalleştirdik. Bunun yanı sıra, kelimeler ve cümleler için AJT Japanese'den furigana da ürettik. Bundan sonra, destenin varsayılan sürümünde kullanılmak üzere temel ipucu içeren cümle kartları CSS'si tasarladık. Son olarak, hataları en aza indirmek için desteyi birden fazla kişi tarafından düzeltme okumasına tabi tuttuk.

“Kaishi” (開始) kelimesi “başlangıç” anlamına gelir. Bunun çok uygun olduğunu düşündük ve bu ismi seçtik. Umarız bu kart destesi, Japonca öğrenme yolculuğunuz için harika bir başlangıç olur.

## Bu deste bittikten sonra ne yapmalıyım?

Henüz başlamadıysanız [madenciliğe başlayın](https://donkuri.github.io/learn-japanese/guide/#consuming-native-content). Madencilik not türlerinin listesi için [buraya](https://github.com/donkuri/japanese-resources/?tab=readme-ov-file#mining) bakın.

## Kart destesinin çevirisi

Bu kart destesini ana dilinize çevirmekle ilgileniyorsanız, lütfen [GitHub izleme sisteminde](https://github.com/donkuri/Kaishi/issues) bir sorun bildirimi oluşturun. Sunum, halihazırda **[Rusça](https://github.com/NeonGooRoo/KaishiRu)**, **[Endonezce](https://ankiweb.net/shared/info/1512066033)**, **[Vietnamca](https://github.com/duy103zxc/kaishi-vi/releases)**, **[Ukraynaca](https://github.com/maksiksq/KaishiUa)**, **[Brezilya Portekizcesi](https://github.com/nonsolvent/Kaishi-pt-BR)**, **[İspanyolca](https://github.com/Dogi5/Kaishi-ESP)**, **[Çince](https://github.com/maimemo/kaishi-zh-cn/)** ve **[Fransızca](https://github.com/khmskhmskhms/kaishi-FR)**.

## Katkıda Bulunanlar

Bu kart destesi aşağıdaki kişilerin yardımıyla hazırlanmıştır:

[栗](https://github.com/donkuri/) - baş mimar, tüm teknik konular, çeviriler, düzeltme okuması

Tyogin - baş mimar, ilk 200 kartın sırasını yeniden düzenledi, cümleleri değiştirdi, düzeltme okuması

shoui - tüm kart destesinin düzeltme okuması, çevirileri düzeltti

Julian - notların eklenmesine yardımcı oldu ve bazı cümle çevirilerini kontrol etti

karifurai - ilk 750 kartın ton vurgusunu doğruladı ve ton notları ekledi

cindsa - son 750 kartın ton vurgusunu doğruladı ve ton notları ekledi

[Kuuube](https://github.com/Kuuuube) - FFmpeg kullanımını önerdi, yukarıdaki Kaishi 1.5k'ya kart aktarma bölümünü yazdı

[stephenmk](https://github.com/stephenmk) - Kaishi 1.5k üzerinde Jmdict Furigana aracını çalıştırarak furigana'yı düzeltti, bkz. v1.3.0

[Kaanium](https://github.com/kaanium) - desteyi yazma versiyonuna dönüştürmek için bir komut dosyası oluşturulmasına yardımcı oldu

[Lars](https://github.com/liarbeast) - [irasutoya](https://www.irasutoya.com/) sitesinden resimler ekledi

Deste oluşturulurken şu araçlar kullanıldı:

[AJT Japanese](https://github.com/Ajatt-Tools/Japanese) - ton vurgusu, furigana ve seslerin bir kısmı bu eklenti kullanılarak oluşturuldu

[FFmpeg](https://ffmpeg.org/) - çeşitli ses dosyalarındaki sessiz kısımları çıkarmak için kullanıldı

[Tenacity](https://tenacityaudio.org/) - çeşitli ses dosyalarındaki kesik sesleri düzenlemek için kullanıldı

Ayrıca, destenin adı da dahil olmak üzere, TMW Discord sunucusundaki birçok üyeden çeşitli fikirler aldık. Cümleler ise Ankiweb'de bulunan çeşitli Core destelerinden alınmıştır.




