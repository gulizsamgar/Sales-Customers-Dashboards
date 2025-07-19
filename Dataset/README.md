# 📦 Projede Kullanılan Veri Setleri: Fact ve Dimension Tablolar

Bu proje kapsamında kullanılan veri setleri, bir satış ve müşteri analiz sisteminin temelini oluşturmaktadır. Veri ambarı yaklaşımıyla düzenlenen bu tablolar, analizler için **fact (olay)** ve **dimension (bağlamsal bilgi)** olarak sınıflandırılmıştır. Aşağıda her bir CSV dosyasının veri ambarı içindeki rolü açıklanmıştır.

---

## 🎯 Fact Table

### [`Orders.csv`](https://github.com/gulizsamgar/Sales-Customers-Dashboards/blob/main/Dataset/Orders.csv)
- **Tanım:** Sipariş detaylarını barındırır (Order ID, Order Date, Ship Date, Customer ID, Product ID, Sales, Quantity, Profit vb.)
- **Fact olma nedeni:** Ölçülebilir metrikleri ve zaman bazlı olayları içerir.
- **Kullanım amacı:** Satış performansı, dönemsel analizler, kar-zarar takibi.
---

## 🧩 Dimension Tables

### [`Customers.csv`](https://github.com/gulizsamgar/Sales-Customers-Dashboards/blob/main/Dataset/Customers.csv)
- **Tanım:** Müşteri bilgilerini içerir (Customer ID, Customer Name).
- **Dimension olma nedeni:** Siparişleri müşteri bazında analiz etmeye yarar.
- **Kullanım amacı:** Müşteri segmentasyonu, müşteri karlılığı analizi.

### [`Products.csv`](https://github.com/gulizsamgar/Sales-Customers-Dashboards/blob/main/Dataset/Products.csv)
- **Tanım:** Ürün bilgilerini içerir (Product ID, Category, Sub-Category, Product Name).
- **Dimension olma nedeni:** Ürün bazlı analizler için bağlamsal veri sağlar.
- **Kullanım amacı:** Kategori trendleri, ürün performans analizi.

### [`Location.csv`](https://github.com/gulizsamgar/Sales-Customers-Dashboards/blob/main/Dataset/Location.csv)
- **Tanım:** Konum bilgilerini içerir (Postal Code, City, State, Region, Country).
- **Dimension olma nedeni:** Sipariş ve müşteri verilerini coğrafi boyutta analiz etmeye yarar.
- **Kullanım amacı:** Bölgesel satış dağılımı, lojistik ve pazarlama planlaması.

---

## 🧠 Not
> Fact tablosu genellikle **çok sayıda kayda** sahipken, dimension tabloları **daha az ama açıklayıcı** kayıtlar içerir. Hepsi birlikte bir **yıldız şeması (star schema)** oluşturarak veri analizi için güçlü bir model sunar.

