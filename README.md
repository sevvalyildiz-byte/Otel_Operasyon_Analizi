\# **Otel Operasyon Analizi**



Bu proje, bir otelin satış, maliyet ve insan kaynakları verilerini kullanarak kapsamlı bir analiz gerçekleştirmektedir. Python ve Pandas ile veri temizliği, özet KPI’lar, segment ve departman analizleri yapılmış, stratejik içgörüler ve aksiyon önerileri raporlanmıştır.



> \\\*\\\*Not:\\\*\\\* Veriler Nuno Antonio, Ana Almeida ve Luis Nunes’in 2019 yılında Data in Brief dergisinde yayınladığı \\\["Otel Rezervasyon Talebi Veri Kümeleri"](https://www.kaggle.com/datasets/jessemostipak/hotel-booking-demand/data) çalışmasından alınmıştır. Satın alma ve maliyet verileri ise \\\*\\\*sentetik olarak oluşturulmuştur\\\*\\\*.  



\---



\## **Temel KPI’lar**

* Toplam Gelir: 2.030.702 TL (iptal edilmeyen rezervasyonlar)
* Ortalama Oda Fiyatı (ADR): 101,54 TL
* İptal Oranı: %37,7
* Tekrar Eden Müşteri Oranı: %3,3
* Ortalama Konaklama Süresi: 3,44 gün



\---



\## **Gelir ve Kanal Analizi**

\- Gelirin %54’ü online seyahat acenteleri üzerinden sağlanıyor. Direct satış sadece %13.

\- Rezervasyonların çoğu bireysel ve paket müşterilerden geliyor; en çok Portekiz, İngiltere ve Fransa’dan misafir var.

\- Aylık gelir trendleri sayesinde yoğun ve sakin dönemler tespit edildi.



\---



\## **Satın Alma ve Maliyet Analizi**

\- En yüksek harcama Mutfak (F\&B) bölümünde, ardından Teknik Servis ve Kat Hizmetleri geliyor.

\- Bu üç bölüm toplam harcamaların yaklaşık %73’ünü oluşturuyor.

\- En kritik maliyet kalemleri toplam harcamaların %60’ını kapsıyor (ör. şampuan, balık, zımba). Böylelikle tedarikçi, ikame veya fiyat talebleri düzenlenmelidir.



\---



\## **İnsan Kaynakları Analizi**

\- Araştırma \& Geliştirme departmanı en kalabalık (961 kişi), İnsan Kaynakları en az çalışanlı (63 kişi).

\- Genel ayrılma oranı %16, Sales departmanında %20,6 ile en yüksek.

\- Gelir/çalışan maliyeti analizinde Araştırma \& Geliştirme en yüksek performans gösteriyor.



\---



\## **Stratejik İçgörüler ve Öneriler**

1\. \*\*Yüksek İptal Oranı (%37,7)\*\*

&#x20;  - Etki: Oda boş kalır, gelir kaybı olur, planlama bozulur

&#x20;  - Aksiyon: Non-refundable fiyatlar, son dakika cezası, overbooking stratejisi



2\. \*\*Online TA Bağımlılığı (%54+)\*\*

&#x20;  - Etki: Komisyon ödemesi → kâr düşüyor

&#x20;  - Aksiyon: Direct booking artırılmalı, web UX, sosyal medya ve sadakat programları



3\. \*\*Direct Kanal Zayıf (%13)\*\*

&#x20;  - Fırsat: Komisyonsuz satış → yüksek kâr

&#x20;  - Aksiyon: Instagram/Google Ads, web UX iyileştirme, repeat customer kampanyası



4\. \*\*Müşteri Sadakati Düşük (%3,3)\*\*

&#x20;  - Etki: Marka bağlılığı yok, her seferinde yeni müşteri maliyeti

&#x20;  - Aksiyon: Loyalty program, e-mail marketing, özel indirimler



5\. \*\*Ana Gelir Kaynağı: Transient Müşteriler (1,6M)\*\*

&#x20;  - Etki: Sadakat düşük, fiyat hassasiyeti yüksek

&#x20;  - Aksiyon: Bu segmenti sadık müşteriye dönüştürmek



6\. \*\*Pazar Analizi (Ülke Bazlı)\*\*

&#x20;  - En büyük pazar: Portekiz (PRT), ardından İngiltere, Fransa, İspanya

&#x20;  - Aksiyon: UK \& FR için özel kampanyalar, dil bazlı reklamlar



\---



\## **Veri Analizi Yaklaşımı**

1. Veri ile doğru hikayeyi anlatmak gerekli
2. KPI’ları belirle, ayrıştırma yöntemi kullan: Gelir, iptal oranı, ADR, repeat rate
3. Her KPI’yı yorumla: İşletmeye etkisi, iyi/kötü durumu
4. Risk ve fırsatları tespit et: Online TA bağımlılığı, Direct kanal, maliyetler
5. Somut aksiyon öner: İptal azaltma, Direct booking, loyalty program
6. Segment ve pazar analizini yap: Müşteri tipi ve ülke bazlı fırsatlar
7. Maliyet ve kaynak verimliliğini kontrol et
8. Stratejik özet oluştur: Gelir artırma + maliyet azaltma, karşılaştırma yöntemi kullanarak yıl/sezona göre yorumlar.
9. **Matris yöntemi** ile; 

Gelir vs Kanal vs Segment

Satır: Müşteri tipi | Sütun: Kanal | Hücre: Gelir/ADR

→ En çok gelir hangi segmentten hangi kanaldan geliyor, tek bakışta.



İptal Oranı Matrisleri

Satır: Rezervasyon tipi | Sütun: Ay/Sezon | Hücre: İptal oranı

→ Hangi kanalda ve hangi ay iptaller yüksek, hızlı tespit.



Personel Verimliliği

Satır: Departman | Sütun: KPI (gelir/çalışan, turnover, maliyet)

→ Hangi departman düşük verimli, kolay görünür.



Pazarlama Kampanyası

Satır: Reklam kanalları | Sütun: KPI (tıklama, rezervasyon, gelir)

→ Hangi kanal en verimli, hemen anlaşılır.



\---



\## **Sonuç**

Bu proje, otelin satış, maliyet ve İK verilerini kullanarak \*\*gelir artırıcı, maliyet düşürücü ve müşteri bağlılığını güçlendirici stratejik içgörüler\*\* sunmaktadır. Grafikler dashboarda dönüştürülerek karar vericiler için hızlı ve etkili bir analiz sağlar.

