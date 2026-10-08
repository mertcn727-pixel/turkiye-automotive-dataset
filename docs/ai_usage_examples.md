# AI İçin Kullanım Örnekleri

Aşağıdaki istemleri Cursor veya başka bir LLM’e doğrudan verebilirsiniz:

1. Toyota Corolla 2018 için en yaygın 5 kronik sorunu ve bunlara uygun parça kodlarını çıkar.
2. 2017-2020 model ticari araçlar için en sık görülen sorunları ve ilgili parça listelerini göster.
3. Tarım makineleri için hidrolik filtre, pompa ve palet parça kodlarını eşleştir.
4. Bu veri setinden sadece 4x4 tarım makinelerini çıkar ve sorun-parça ilişkisini tablo hale getir.
5. Oto bakım raporu oluştur: araç, sorun, parça, maliyet ve neden alanlarını doldur.

Yapılandırılmış istek örneği:
- vehicle_id
- brand
- model
- year
- category
- issue_category
- part_name
- oem_code
- aftermarket_code

AI için optimize edilmiş çıktı bekleyin:
- markdown tablo
- JSON array
- CSV snippet
- araç bazlı özet rapor

Bu repo, Cursor’a verildiğinde aşağıdaki işlemleri yapabilir:
- araç filtreleme
- sorun sınıflandırma
- parça kodu eşleme
- OEM/muadil kod üretimi
- bakım ve öncelik çıktısı
