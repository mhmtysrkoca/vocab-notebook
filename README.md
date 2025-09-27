# vocab-notebook
# Almanca Kelime Defteri

Türkçe → Almanca kişisel kelime defteri. Aynı Türkçe kelimeyi kaç kez girersen gir — **tek kayıt** tutulur. Liste her zaman **alfabetik** sıralıdır. Canlı **arama**, satırdan **düzenle/sil**, **CSV içe/dışa aktarım** ve **localStorage** ile kalıcı kayıt içerir.

**Canlı demo:** `https://mhmtysrkoca.github.io/vocab-notebook/`  
*(Farklı repo adı kullandıysan: `https://<kullanıcı-adın>.github.io/<repo-adı>/`)*

---

## Özellikler
- **Tekil kayıt (dupe engelleme):** Aynı Türkçe kelime tekrar yazıldığında **güncellenir**, yeni satır eklenmez.
- **Alfabetik sıralama:** Liste daima **Türkçe kelimeye** göre sıralıdır (TR dil kuralları ile).
- **Arama:** Türkçe, Almanca ve Not alanlarında canlı arama.
- **Düzenle/Sil:** Satırdaki “Düzenle” butonu formu doldurur; “Ekle/Güncelle” kaydeder.
- **Kalıcı kayıt:** Tarayıcı **localStorage**’a kaydeder (çevrimdışı da çalışır).
- **CSV içe/dışa aktar:** Dışa aktar: `vocab.csv`. İçe aktar: mevcut listeyle **birleştirerek (upsert)** ekler.

---

## Hızlı Başlangıç
1. Bu repoda `index.html` vardır (tek dosya).  
2. GitHub Pages’i aç: **Settings → Pages → Deploy from a branch → main / /** → **Save**.  
3. Tarayıcıda aç, kelimeni gir: **Türkçe** → **Almanca** (+ opsiyonel **Not**).  
4. **Ekle/Güncelle** butonuna bas.

> **Klavye kısayolları:**  
> - `Enter` (Türkçe alanında): Almanca alanına geçer.  
> - `Enter` (Almanca/Not alanında): Kaydı Ekle/Güncelle.

---

## Kullanım Detayları
- **Tekilleştirme nasıl çalışır?**  
  Türkçe kelime, küçük harfe çevrilip aksan/işaretlerden arındırılarak “anahtar” yapılır. Aynı anahtarla eklenen yeni kayıt, mevcut olanı **günceller**.
- **Sıralama**  
  `tr-TR` yerel ayarına göre, duyarlılık “base” olacak şekilde alfabetik sıralama yapılır.
- **Arama**  
  Türkçe/Almanca/Not alanlarında normalleştirilmiş metin üzerinde canlı filtreleme.

---

## CSV İçe/Dışa Aktarım
- **Dışa aktarım** formatı (başlık satırıyla):
