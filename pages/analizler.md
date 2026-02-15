---
layout: page
title: Analizler
permalink: /analizler/
---

## Yıllara Göre Belge/Görsel Grafiği

Bu grafik, koleksiyondaki eserlerin yıllara göre dağılımını gösterir. Alt kısımdaki çubuğu kullanarak belirli bir döneme odaklanabilirsiniz.

<div style="width: 100%; height: 500px; border: 1px solid #ddd; border-radius: 5px; overflow: hidden; margin-bottom: 40px;">
    <iframe src="/koleksiyonum/assets/vis/analiz_yillar.html" 
            width="100%" 
            height="100%" 
            frameborder="0"
            style="display: block;">
    </iframe>
</div>

---

## Konu İlişki Ağı (Network Analizi)

Aşağıdaki interaktif ağ haritası, bu koleksiyonda en sık geçen kavramları ve bunların yoğunluğunu gösterir. 
- **Kullanım:** Yuvarlakları (düğümleri) tutup sürükleyebilirsiniz. 
- **Detay:** Fare ile üzerlerine gelerek kaç kayıtta geçtiğini görebilirsiniz.

<div style="width: 100%; height: 650px; border: 1px solid #ddd; border-radius: 5px; overflow: hidden;">
    <iframe src="/koleksiyonum/assets/vis/analiz_ag.html" 
            width="100%" 
            height="100%" 
            frameborder="0"
            style="display: block;">
    </iframe>
</div>


Mehmet Genç'in entelektüel dünyasını, kurumsal ilişkilerini ve eser üretimini inceleyen interaktif ağ analizleri.
<div class="alert alert-info">
  <strong>İpucu:</strong> Grafikler interaktiftir. Düğümleri (yuvarlakları) tutup sürükleyebilir, fare tekerleği ile yakınlaştırıp uzaklaştırabilirsiniz.
</div>

## 1. Sosyal Ağ: Kişiler
Mehmet Genç'in akademik hayatı boyunca etkileşimde bulunduğu, referans verdiği veya ortak çalışmalar yürüttüğü kişiler.
*(Not: Veri girişini yapan kişiler ve kurumsal isimler filtrelenmiştir.)*

<div style="width: 100%; height: 650px; border: 1px solid #ddd; border-radius: 5px; overflow: hidden; margin-bottom: 50px;">
    <iframe src="/koleksiyonum/assets/vis/network_kisi_clean_son.html" 
            width="100%" 
            height="100%" 
            frameborder="0"
            style="display: block;">
    </iframe>
</div>

---

## 2. Kurumsal Ağ
Mehmet Genç ile adı geçen üniversiteler, vakıflar, dernekler ve araştırma merkezleri ile olan bağlantılar.

<div style="width: 100%; height: 650px; border: 1px solid #ddd; border-radius: 5px; overflow: hidden; margin-bottom: 50px;">
    <iframe src="/koleksiyonum/assets/vis/network_kurum_final_son.html" 
            width="100%" 
            height="100%" 
            frameborder="0"
            style="display: block;">
    </iframe>
</div>

---

## 3. Eserlerin Tasnifi
Koleksiyonda yer alan ve **"Eserleri"** başlığı altında toplanan çalışmaların türlerine (Kitap, Makale, Konferans vb.) göre dağılımı.

<div style="width: 100%; height: 800px; border: 1px solid #ddd; border-radius: 5px; overflow: hidden;">
    <iframe src="/koleksiyonum/assets/vis/network_eser_v2.html" 
            width="100%" 
            height="100%" 
            frameborder="0"
            style="display: block;">
    </iframe>
</div>

<br>
*Not: Veriler koleksiyon metadata dosyasından otomatik olarak derlenmiştir.*
