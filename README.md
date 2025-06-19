# Modern Anime Kişilik Testi

Bu proje, kullanıcıların anime zevklerine ve tercihlerine göre kişiliklerini analiz eden, modern, interaktif ve dinamik bir web uygulamasıdır. Kullanıcılar 20 soruya cevap vererek kendilerine en uygun anime türünü, karakter profilini ve bir anime önerisi alırlar.

---

## ✨ Özellikler

- **Dinamik Sorular ve Görseller:** Her soru için ilgili anime görseli, [AniList GraphQL API](https://anilist.gitbook.io/anilist-apiv2-docs/) üzerinden anlık olarak çekilir. Bu sayede test daha canlı ve ilgi çekici hale gelir.
- **Gelişmiş Puanlama Sistemi:** Test sadece en çok seçilen şıkka göre sonuç vermez. Birincil ve ikincil kişilik tiplerini analiz ederek daha isabetli ve özelleştirilmiş **kombinasyon sonuçları** (örn: Aksiyon + Felsefe) üretir.
- **Modern ve Duyarlı Tasarım:** Koyu tema, CSS değişkenleri, `flexbox` ve akıcı animasyonlar kullanılarak hem masaüstü hem de mobil cihazlarda harika bir kullanıcı deneyimi sunar.
- **İlerleme Çubuğu:** Test boyunca kullanıcının ilerlemesini gösteren dinamik bir ilerleme çubuğu bulunur.
- **Bağımlılıksız (Zero-Dependency):** Proje, herhangi bir harici kütüphane veya framework'e ihtiyaç duymadan, saf (Vanilla) HTML, CSS ve JavaScript ile oluşturulmuştur.

---

## 🛠️ Kullanılan Teknolojiler

- **HTML5:** Projenin temel iskeleti.
- **CSS3:**
  - **CSS Değişkenleri (Variables):** Kolay tema yönetimi için.
  - **Flexbox:** Modern ve esnek sayfa düzeni için.
  - **Transitions & Animations:** Akıcı ve pürüzsüz bir kullanıcı deneyimi için.
- **Vanilla JavaScript (ES6+):**
  - **DOM Manipülasyonu:** Testin tüm interaktif mantığı.
  - **Fetch API & Async/Await:** AniList API'sinden asenkron veri çekmek için.
  - **Web Audio API:** UI ses efektleri üretmek için.
- **AniList GraphQL API:** Anime görsellerini ve verilerini dinamik olarak sağlamak için.

---

## 🧠 Nasıl Çalışır?

1.  **Sorular ve Puanlama:** Her sorudaki seçenekler dört ana kategoriye ayrılmıştır:
    -   `A`: Derinlik, Felsefe, Dram (Seinen)
    -   `B`: Aksiyon, Macera, Güç (Shounen)
    -   `C`: Komedi, Eğlence, Günlük Hayat (Slice of Life/Comedy)
    -   `D`: Romantizm, Duygusallık, İlişkiler (Romance)
2.  **Puan Toplama:** Kullanıcının her cevabı, ilgili kategorideki (`A`, `B`, `C`, `D`) puanı bir artırır.
3.  **Sonuç Analizi:** Test bittiğinde:
    -   En yüksek puanı alan tip **"birincil"**, ikinci en yüksek puanı alan ise **"ikincil"** tip olarak belirlenir.
    -   Eğer ikincil tipin puanı, birincil tipin puanının belirli bir oranından fazlaysa (kodda `> primaryScore / 2`), bu iki tip birleştirilerek daha spesifik bir kombinasyon sonucu (örneğin `AB`, `AC`, `CD` vb.) oluşturulur.
    -   Bu sonuca göre kullanıcıya özel bir kişilik tanımı, karakter profili ve anime önerisi sunulur.

---

## 🚀 Kurulum ve Kullanım

Proje herhangi bir derleme veya kurulum adımı gerektirmez.

1.  Depoyu klonlayın:
    ```bash
    git clone https://github.com/KerimDemirkaynak/AnimeTesti.git
    ```
2.  Proje klasörüne gidin:
    ```bash
    cd REPOADINIZ
    ```
3.  `index.html` dosyasını favori web tarayıcınızda açın. Hepsi bu kadar!

---

## 📜 Lisans

Bu proje [MIT Lisansı](LICENSE) ile lisanslanmıştır. Daha fazla bilgi için `LICENSE` dosyasına göz atın.

---

## 🙏 Teşekkür

-   Harika anime veritabanı ve API'si için [AniList](https://anilist.co/)'e teşekkürler.
-   İlham veren tüm anime ve mangakalara.

---
