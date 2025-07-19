# 📊 Veri Setleri Sınıflandırması: Fact ve Dimension Tablolar

Veri ambarı mantığında tablolar genellikle iki ana gruba ayrılır: **Fact (gerçekleşen olaylar)** ve **Dimension (bağlamsal detaylar)**.

---

## 🎯 Fact Table

### `Orders.csv`
- **Tanım:** Sipariş detaylarını barındırır (müşteri, ürün, tarih, tutar).
- **Fact olma nedeni:** Ölçülebilir metrikleri içerir (sipariş tutarı, adet, tarih).
- **Kullanım amacı:** İşlem hacmi, dönemsel analizler ve performans ölçümleri.

---

## 🧩 Dimension Tables

### `Customers.csv`
- **Tanım:** Müşteri bilgilerinin yer aldığı tablo (Customer ID;Customer Name).
- **Dimension olma nedeni:** Siparişleri bağlamsal olarak anlamlandırmak için kullanılır.
- **Kullanım amacı:** Müşteri segmentasyonu.

### `Products.csv`
- **Tanım:** Ürün özelliklerini içerir (isim, kategori, marka, fiyat).
- **Dimension olma nedeni:** Sipariş edilen ürünleri tanımlamak için kullanılır.
- **Kullanım amacı:** Kategori bazlı satış analizleri, ürün performansı karşılaştırmaları.

### `Location.csv`
- **Tanım:** Konum bilgilerini içerir (şehir, ülke, posta kodu).
- **Dimension olma nedeni:** Müşteri ve siparişlerin coğrafi yerleşimini anlamlandırır.
- **Kullanım amacı:** Bölgesel satış trendleri, lojistik değerlendirmeleri.

---

## 🧠 Not
> Fact tablosu genellikle **çok sayıda kayda** sahipken, dimension tabloları **daha az ama açıklayıcı** kayıtlar içerir. Hepsi birlikte bir **yıldız şeması (star schema)** oluşturarak veri analizi için güçlü bir model sunar.

