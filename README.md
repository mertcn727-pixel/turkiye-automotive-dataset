# Türkiye Otomotiv Veri Seti - Başlangıç Şablonu

Bu repo, Türkiye’de araçlar için kronik sorunlar, parça bilgileri ve araç/marka/model eşiği içeren AI tarafından kullanılabilir bir başlangıç veri seti sunar.

Amaç:
- araç bazlı veri düzeni kurmak
- marka/model/yıl/motor bazında ayrıştırma sağlamak
- kronik sorunlar ve parça kodlarını eşlemek
- yapay zekaya verildiğinde araç bazlı rapor üretimini kolaylaştırmak

Klasör yapısı:
- `data/vehicles.csv` → araç tanımları
- `data/chronic_issues.csv` → araçlara ait kronik sorunlar
- `data/parts.csv` → parça master listesi
- `data/vehicle_part_map.csv` → araç ve parça eşleştirmesi
- `docs/sample_report.md` → örnek araç raporu
- `schema/vehicle_schema.json` → veri yapısı tanımı

Not:
- Bu örnek veri seti, örnek ve eğitim amaçlıdır.
- Gerçek üretim ortamında OEM kodları, katalog eşleşmeleri ve bakım servis kayıtları ile zenginleştirilmelidir.
- Veri kaynakları için yerli kataloglar, OEM servisler, VIN sorgulama servisleri ve ticari kataloglar kullanılmalıdır.

Önerilen kullanım:
1. `vehicles.csv` içindeki araç kimlikleri ile `parts.csv` eşleştirilir.
2. `chronic_issues.csv` ile araçların yaygın sorunları çıkarılır.
3. Her araç için bir özet rapor oluşturulur.
4. Bu repo, LLM / AI sistemlerine veri besleme için hazır hale getirilir.

Uygulama örneği:
- marka: Toyota
- model: Corolla
- yıl: 2018
- motor: 1.8L
- sorunlar: yağ tüketimi, süspansiyon aşınması, su pompası arızası
- parçalar: yağ filtresi, ön fren seti, su pompası, amortisör
