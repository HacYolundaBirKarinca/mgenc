---
title: Ana Sayfa
layout: page
permalink: /
---

<link rel="preconnect" href="https://fonts.googleapis.com">
<link href="https://fonts.googleapis.com/css2?family=Cormorant+Garamond:ital,wght@0,300;0,400;0,600;1,300;1,400&family=Crimson+Pro:ital,wght@0,300;0,400;1,300;1,400&display=swap" rel="stylesheet">
<style>
/* ── CB override ── */
#maincontent > .container > h1,
#maincontent > .container > h2:first-child { display: none !important; }
#maincontent > .container {
  max-width: 100% !important;
  padding: 0 !important;
  margin: 0 !important;
}
/* CB site başlığı ("Hac Yolunda..." + "Dijital Biyografi") bölümünü gizle */
#site-title, .site-title-section, header.site-header,
.jumbotron.py-3, #jumbotron,
main > div > .jumbotron,
body > header { display: none !important; }

/* ═══════════════════════════════════════════
   MEHMET GENÇ — ANA SAYFA TASARIMI
   CollectionBuilder menü/header korunuyor
═══════════════════════════════════════════ */
:root {
  --ink:      #18120c;
  --parchment:#f5efe2;
  --cream:    #faf6ed;
  --warm:     #e8ddc8;
  --rust:     #7a2e12;
  --gold:     #a8821e;
  --gold-lt:  #c9a84c;
  --muted:    #7a6e5e;
  --border:   #d8cdb8;
  --card:     #fdfaf3;
}

#mg-home * { box-sizing: border-box; }
#mg-home {
  font-family: 'Crimson Pro', Georgia, serif;
  color: var(--ink);
  /* Bootstrap container'ının padding/max-width'ini kır */
  margin-left: -15px;
  margin-right: -15px;
  margin-top: -1rem;
  width: calc(100% + 30px);
  overflow-x: hidden;
}

/* Google Fonts */


/* ── HERO ── */
.mghero {
  background: var(--ink);
  padding: 2.5rem 2rem 3rem;
  display: flex;
  flex-direction: column;
  justify-content: center;
}
@media (min-width: 768px) {
  .mghero { padding: 3rem 4rem 4rem; }
}
.mghero-left {
  max-width: 800px;
}

.mghero-title {
  font-family: 'Cormorant Garamond', serif;
  font-size: clamp(2.2rem, 4vw, 3.2rem);
  font-weight: 300;
  color: #f0e8d8;
  line-height: 1.2;
  margin-bottom: 0.4rem;
}
.mghero-title em { font-style: italic; color: var(--gold-lt); }

.mghero-bio {
  font-size: 1rem;
  color: rgba(240,232,216,0.8);
  line-height: 1.75;
  max-width: 480px;
  margin-bottom: 0.6rem;
}
.mghero-bio strong { color: var(--gold-lt); font-weight: 400; }
.mghero-dates {
  font-size: 0.82rem;
  color: rgba(240,232,216,0.4);
  letter-spacing: 0.06em;
  margin-bottom: 2rem;
}
.mghero-cta {
  display: flex;
  gap: 1rem;
  flex-wrap: wrap;
  margin-bottom: 3rem;
}
.btn-gold {
  background: var(--gold);
  color: var(--ink);
  padding: 0.7rem 1.6rem;
  border-radius: 3px;
  text-decoration: none;
  font-size: 0.88rem;
  font-weight: 600;
  letter-spacing: 0.04em;
  transition: background .2s;
}
.btn-gold:hover { background: var(--gold-lt); text-decoration: none; color: var(--ink); }
.btn-outline-light {
  border: 1px solid rgba(201,168,76,0.5);
  color: rgba(240,232,216,0.75);
  padding: 0.7rem 1.6rem;
  border-radius: 3px;
  text-decoration: none;
  font-size: 0.88rem;
  transition: border-color .2s, color .2s;
}
.btn-outline-light:hover { border-color: var(--gold-lt); color: #f0e8d8; text-decoration: none; }

.mghero-stats {
  display: flex;
  gap: 2.5rem;
  border-top: 1px solid rgba(201,168,76,0.2);
  padding-top: 1.5rem;
}
.stat-num { font-family: 'Cormorant Garamond', serif; font-size: 1.8rem; font-weight: 300; color: var(--gold-lt); }
.stat-lbl { font-size: 0.72rem; color: rgba(240,232,216,0.45); text-transform: uppercase; letter-spacing: 0.08em; }

/* Hero sağ — mozaik */


/* ── ORTAK SECTION ── */
.mg-section { padding: 5rem 0; }
.mg-section-inner { max-width: 1100px; margin: 0 auto; padding: 0 2rem; }
.mg-section-label {
  font-size: 0.68rem; letter-spacing: 0.18em; text-transform: uppercase;
  color: var(--gold); margin-bottom: 0.5rem;
}
.mg-section-title {
  font-family: 'Cormorant Garamond', serif;
  font-size: clamp(1.6rem, 3vw, 2.2rem);
  font-weight: 300;
  color: var(--rust);
  margin-bottom: 0.5rem;
  line-height: 1.3;
}
.mg-section-sub { color: var(--muted); font-size: 1rem; margin-bottom: 2.5rem; }

/* ── BİYOGRAFİ ── */
.mg-bio { background: var(--cream); }
.mg-bio-grid {
  display: grid;
  grid-template-columns: 260px 1fr;
  gap: 4rem;
  align-items: start;
}
.mg-bio-portrait-frame {
  border: 1px solid var(--border);
  padding: 6px;
  background: #fff;
  box-shadow: 4px 6px 20px rgba(0,0,0,0.08);
}
.mg-bio-portrait-frame img {
  width: 100%; display: block;
  filter: sepia(0.08);
}
.mg-bio-caption {
  text-align: center;
  font-size: 0.78rem;
  color: var(--muted);
  margin-top: 0.5rem;
  font-style: italic;
}
.mg-dates-strip {
  display: flex;
  gap: 2rem;
  background: var(--parchment);
  border: 1px solid var(--border);
  padding: 1rem 1.5rem;
  border-radius: 4px;
  margin-bottom: 1.5rem;
}
.mg-date-val { font-family: 'Cormorant Garamond', serif; font-size: 1.4rem; color: var(--rust); }
.mg-date-lbl { font-size: 0.75rem; color: var(--muted); }
.mg-bio-text p { color: #3a2e24; line-height: 1.8; margin-bottom: 1rem; font-size: 1rem; }
.mg-bio-text strong { font-weight: 600; color: var(--ink); }
.mg-blockquote {
  border-left: 3px solid var(--gold);
  padding: 0.8rem 1.2rem;
  margin: 1.5rem 0;
  background: var(--parchment);
  font-style: italic;
  font-size: 1rem;
  color: #3a2e24;
  line-height: 1.7;
}
.mg-blockquote cite { display: block; font-size: 0.8rem; color: var(--muted); margin-top: 0.4rem; font-style: normal; }
.btn-rust {
  display: inline-block;
  border: 1px solid var(--rust);
  color: var(--rust);
  padding: 0.55rem 1.3rem;
  border-radius: 3px;
  font-size: 0.88rem;
  text-decoration: none;
  transition: background .2s, color .2s;
}
.btn-rust:hover { background: var(--rust); color: #fff; text-decoration: none; }

/* ── PORTAL KAPILAR ── */
.mg-portals { background: var(--parchment); }
.mg-portal-grid { display: grid; grid-template-columns: repeat(3, 1fr); gap: 1.5rem; }
.mg-portal-card {
  background: #fff;
  border: 1px solid var(--border);
  border-top: 3px solid var(--gold);
  padding: 2rem 1.8rem;
  border-radius: 3px;
  text-decoration: none;
  color: var(--ink);
  transition: transform .2s, box-shadow .2s;
  display: block;
}
.mg-portal-card:hover {
  transform: translateY(-4px);
  box-shadow: 0 8px 24px rgba(0,0,0,0.1);
  text-decoration: none; color: var(--ink);
}
.mg-portal-icon { font-size: 2rem; margin-bottom: 0.8rem; }
.mg-portal-name {
  font-family: 'Cormorant Garamond', serif;
  font-size: 1.3rem; color: var(--rust);
  margin-bottom: 0.7rem;
}
.mg-portal-desc { font-size: 0.9rem; color: var(--muted); line-height: 1.65; margin-bottom: 1rem; }
.mg-portal-tags { display: flex; flex-wrap: wrap; gap: 0.4rem; margin-bottom: 1.2rem; }
.mg-portal-tag {
  font-size: 0.72rem; color: var(--rust);
  border: 1px solid rgba(122,46,18,0.25);
  border-radius: 20px; padding: 2px 9px;
  background: rgba(122,46,18,0.05);
}
.mg-portal-count {
  display: flex; justify-content: space-between; align-items: center;
  font-size: 0.82rem; color: var(--muted);
  border-top: 1px solid var(--border); padding-top: 0.8rem;
}
.mg-portal-arrow { color: var(--gold); font-size: 1rem; }

/* ── ZAMANÇİZGİSİ ── */
.mg-timeline { background: #16120e; }
.mg-timeline .mg-section-title { color: var(--gold-lt); }
.mg-timeline .mg-section-sub { color: rgba(240,232,216,0.5); }
.mg-timeline .mg-section-label { color: rgba(201,168,76,0.7); }
.mg-tl-scroll {
  display: flex;
  gap: 0;
  overflow-x: auto;
  padding-bottom: 1rem;
  scrollbar-width: thin;
  scrollbar-color: var(--gold) transparent;
}
.mg-tl-scroll::-webkit-scrollbar { height: 4px; }
.mg-tl-scroll::-webkit-scrollbar-track { background: transparent; }
.mg-tl-scroll::-webkit-scrollbar-thumb { background: var(--gold); border-radius: 2px; }
.mg-decade {
  min-width: 200px;
  border-left: 1px solid rgba(201,168,76,0.25);
  padding: 0 1.5rem 1.5rem;
  position: relative;
}
.mg-decade-label {
  font-family: 'Cormorant Garamond', serif;
  font-size: 2rem; font-weight: 300;
  color: rgba(201,168,76,0.35);
  margin-bottom: 1rem;
}
.mg-decade::before {
  content: '';
  position: absolute; top: 0; left: -5px;
  width: 9px; height: 9px;
  background: var(--gold); border-radius: 50%;
}
.mg-tl-event {
  font-size: 0.82rem;
  color: rgba(240,232,216,0.6);
  line-height: 1.5;
  margin-bottom: 0.6rem;
  padding-left: 0.5rem;
}
.mg-tl-event strong { color: var(--gold-lt); display: block; font-weight: 400; font-size: 0.75rem; }
.mg-tl-footer {
  margin-top: 2.5rem;
  text-align: center;
  color: rgba(240,232,216,0.4);
  font-size: 0.9rem;
  display: flex;
  flex-direction: column;
  align-items: center;
  gap: 1rem;
}
.btn-outline-gold {
  display: inline-block;
  border: 1px solid rgba(168,130,30,0.4);
  color: #c8b98a;
  padding: 0.55rem 1.3rem;
  border-radius: 3px;
  font-size: 0.85rem;
  text-decoration: none;
  transition: border-color .2s, color .2s;
}
.btn-outline-gold:hover { border-color: var(--gold-lt); color: var(--gold-lt); text-decoration: none; }

/* ── KONU BULUTU ── */
.mg-topics { background: var(--cream); }
.mg-topic-cloud { display: flex; flex-wrap: wrap; gap: 0.7rem; }
.mg-topic-tag {
  text-decoration: none;
  border-radius: 3px;
  font-family: 'Cormorant Garamond', serif;
  transition: background .2s, color .2s;
  border: 1px solid var(--border);
  color: var(--ink);
  background: #fff;
}
.mg-topic-tag:hover { background: var(--rust); color: #fff; border-color: var(--rust); text-decoration: none; }
.mg-topic-tag.large { font-size: 1.4rem; padding: 0.4rem 1.1rem; }
.mg-topic-tag.medium { font-size: 1.1rem; padding: 0.3rem 0.9rem; }
.mg-topic-tag.small { font-size: 0.88rem; padding: 0.25rem 0.75rem; }

/* ── VERİ KARTLARI ── */
.mg-data { background: var(--parchment); }
.mg-data-grid { display: grid; grid-template-columns: repeat(4, 1fr); gap: 1rem; }
.mg-data-card {
  background: #fff;
  border: 1px solid var(--border);
  padding: 2rem 1.5rem;
  text-align: center;
  border-radius: 3px;
  text-decoration: none;
  color: var(--ink);
  transition: border-color .2s, box-shadow .2s;
  display: block;
}
.mg-data-card:hover { border-color: var(--gold); box-shadow: 0 4px 12px rgba(0,0,0,0.07); text-decoration: none; }
.mg-data-icon { font-size: 1.8rem; margin-bottom: 0.5rem; }
.mg-data-num {
  font-family: 'Cormorant Garamond', serif;
  font-size: 2.4rem; font-weight: 300; color: var(--rust);
  line-height: 1;
}
.mg-data-label { font-size: 0.8rem; color: var(--muted); margin-top: 0.3rem; text-transform: uppercase; letter-spacing: 0.08em; }

/* reveal devre dışı */

/* ── HERO FOTOĞRAF CROSSFADE (5 fotoğraf) ── */
.mghero-photo-wrap {
  position: relative;
  background: #0e0c09;
  overflow: hidden;
  border-left: 1px solid rgba(201,168,76,0.15);
}
.mghero-photo {
  position: absolute;
  inset: 0;
  width: 100%;
  height: 100%;
  object-fit: cover;
  object-position: center top;
  display: block;
  opacity: 0;
}
/* Her fotoğraf 25s döngüde 5s görünür, 1s geçiş */
/* Sıra: p1 → p2 → p3 → p4 → p5 → p1 ... */
.photo-1 { animation: fade5 25s 0s  infinite; }
.photo-2 { animation: fade5 25s 5s  infinite; }
.photo-3 { animation: fade5 25s 10s infinite; }
.photo-4 { animation: fade5 25s 15s infinite; }
.photo-5 { animation: fade5 25s 20s infinite; }
@keyframes fade5 {
  0%   { opacity: 0; }
  4%   { opacity: 1; }
  20%  { opacity: 1; }
  24%  { opacity: 0; }
  100% { opacity: 0; }
}

/* ── RESPONSIVE ── */
@media (max-width: 900px) {
  .mghero {
    grid-template-columns: 1fr !important;
    min-height: auto !important;
  }
  .mghero-left {
    padding: 2rem 1.5rem 2rem !important;
  }
  .mghero-photo-wrap {
    height: 280px;
    border-left: none !important;
    border-top: 1px solid rgba(201,168,76,0.15);
  }
  .mghero-photo { object-position: center 20%; }
  .mg-bio-grid { grid-template-columns: 1fr; }
  .mg-portal-grid { grid-template-columns: 1fr; }
  .mg-data-grid { grid-template-columns: repeat(2,1fr); }
}
@media (max-width: 600px) {
  .mghero-stats { gap: 1.5rem; }
  .mg-data-grid { grid-template-columns: 1fr 1fr; }
}
</style>

<div id="mg-home">

<!-- ════════ HERO ════════ -->
<section class="mghero" style="display:grid;grid-template-columns:1fr 1fr;min-height:85vh;overflow:hidden;position:relative;">
  <div class="mghero-left" style="background:#18120c;padding:2.5rem 3rem 3rem;display:flex;flex-direction:column;justify-content:center;">
    <h1 class="mghero-title">
      Hac Yolunda<br><em>Bir Karınca</em>
    </h1>
    <p class="mghero-bio">
      <strong>Osmanlı iktisat tarihi</strong>nin en özgün seslerinden biri. Yarım asrı aşan akademik yolculuğunu, yazılı eserlerini, konferanslarını ve yaşamının izlerini bir araya getiren dijital koleksiyon.
    </p>
    <p class="mghero-dates">1934, Artvin &nbsp;·&nbsp; 2021, İstanbul</p>
    <div class="mghero-cta">
      <a href="https://hacyolundabirkarinca.github.io/mgenc/browse.html" class="btn-gold">Koleksiyonu Keşfet →</a>
      <a href="https://hacyolundabirkarinca.github.io/mgenc/biyografi.html" class="btn-outline-light">Hayatını Oku</a>
      <a href="https://hacyolundabirkarinca.github.io/mgenc/about.html" class="btn-outline-light">Portal Hakkında</a>
      <a href="https://hacyolundabirkarinca.github.io/mgenc/katki.html" class="btn-outline-light">Siz de Paylaşın</a>
    </div>
    <div class="mghero-stats">
      <div><div class="stat-num">229</div><div class="stat-lbl">Akademik</div></div>
      <div><div class="stat-num">114</div><div class="stat-lbl">Görsel</div></div>
      <div><div class="stat-num">88</div><div class="stat-lbl">Biyografik</div></div>
      <div><div class="stat-num">53</div><div class="stat-lbl">Video</div></div>
    </div>
  </div>
  <div class="mghero-photo-wrap">
    <img class="mghero-photo photo-1"
      src="https://hacyolundabirkarinca.github.io/mgenc/objects/dunyabizim3.jpg"
      alt="Mehmet Genç">
    <img class="mghero-photo photo-2"
      src="https://hacyolundabirkarinca.github.io/mgenc/objects/kenanyildiz.jpg"
      alt="Mehmet Genç arşivde">
    <img class="mghero-photo photo-3"
      src="https://hacyolundabirkarinca.github.io/mgenc/objects/yedikıta.jpg"
      alt="Mehmet Genç kitaplığında">
    <img class="mghero-photo photo-4"
      src="https://hacyolundabirkarinca.github.io/mgenc/objects/odessa2.jpg"
      alt="Mehmet Genç Odessa'da">
    <img class="mghero-photo photo-5"
      src="https://hacyolundabirkarinca.github.io/mgenc/objects/sakul.jpg"
      alt="Mehmet Genç çalışırken">
  </div>
</section>

<!-- ════════ BİYOGRAFİ ════════ -->
<section class="mg-section mg-bio">
  <div class="mg-section-inner">
    <div class="mg-bio-grid">
      <div>
        <div class="mg-bio-portrait-frame">
          <img src="https://hacyolundabirkarinca.github.io/mgenc/assets/img/derivatives/square/solak_sm.jpg"
               onerror="this.style.display='none'" alt="Mehmet Genç">
        </div>
        <p class="mg-bio-caption" style="font-size:1.4rem;font-family:'Cormorant Garamond',serif;font-weight:400;color:var(--rust);margin-top:1rem;letter-spacing:0.02em;">Mehmet Genç (1934–2021)</p>
      </div>
      <div>
        <div class="mg-section-label">Hayatı</div>
        <h2 class="mg-section-title">Osmanlı'nın İktisat Tarihçisi</h2>
        <div class="mg-dates-strip">
          <div><div class="mg-date-val">1934</div><div class="mg-date-lbl">Doğum · Artvin, Arhavi</div></div>
          <div><div class="mg-date-val">1975–</div><div class="mg-date-lbl">Akademik Kariyer</div></div>
          <div><div class="mg-date-val">2021</div><div class="mg-date-lbl">Vefat · İstanbul</div></div>
        </div>
        <div class="mg-bio-text">
          <p>Mehmet Genç, Osmanlı iktisat tarihini tek başına yeniden çerçevelemiş bir âlimdir. Yıllarca süren arşiv çalışmasından damıttığı <strong>iaşecilik, fiskalizm ve gelenekçilik</strong> ilkeleri, Osmanlı ekonomik düşüncesini anlamlandırmak için bir kuşağın başvurduğu temel kavramsal araçlara dönüştü.</p>
          <p>İstanbul Üniversitesi ve İstanbul Şehir Üniversitesi'ndeki onlarca yıllık hocalık hayatı boyunca yetiştirdiği öğrenciler, arşiv okumasına getirdiği titizliği farklı kuşaklara taşımaya devam ediyor.</p>
        </div>
        <blockquote class="mg-blockquote">
          "Osmanlı arşivi bana düşünmekten çok görmek için bir fırsat verdi. Ben hep belgenin kendisinin ne söylediğini dinlemeye çalıştım."
          <cite>— Mehmet Genç</cite>
        </blockquote>
        <a href="https://hacyolundabirkarinca.github.io/mgenc/biyografi.html" class="btn-rust">Hayat hikâyesini okuyun →</a>
      </div>
    </div>
  </div>
</section>

<!-- ════════ ZAMANÇİZGİSİ ════════ -->
<section class="mg-section mg-timeline">
  <div class="mg-section-inner">
    <div class="mg-section-label">Kronoloji</div>
    <h2 class="mg-section-title">Kronolojiden Notlar</h2>
    <p class="mg-section-sub">1970'lerden 2020'lere uzanan akademik yolculuktan öne çıkan anlar.</p>

    <div class="mg-tl-scroll" id="mgTimeline">
      <div class="mg-decade">
        <div class="mg-decade-label">1970</div>
        <div class="mg-tl-event"><strong>1973</strong>Malikane Sistemi Semineri</div>
        <div class="mg-tl-event"><strong>1975</strong>İlk bildiri: Osmanlı Maliyesinde Malikâne</div>
        <div class="mg-tl-event"><strong>1977</strong>Himayeci Gümrük Semineri, Hacettepe</div>
      </div>
      <div class="mg-decade">
        <div class="mg-decade-label">1980</div>
        <div class="mg-tl-event"><strong>1981</strong>18. Yy. Mali Verileri Makalesi</div>
        <div class="mg-tl-event"><strong>1983</strong>Princeton & Münih konferansları</div>
        <div class="mg-tl-event"><strong>1987</strong>Cambridge'de kitap bölümü yayını</div>
        <div class="mg-tl-event"><strong>1989</strong>Osmanlı İktisadî Dünya Görüşü İlkeleri</div>
      </div>
      <div class="mg-decade">
        <div class="mg-decade-label">1990</div>
        <div class="mg-tl-event"><strong>1990</strong>Harvard, Columbia, Binghamton turu</div>
        <div class="mg-tl-event"><strong>1995</strong>Heidelberg Üniversitesi konferansı</div>
        <div class="mg-tl-event"><strong>1997</strong>Japonya: Tokyo & Yamagata</div>
        <div class="mg-tl-event"><strong>1999</strong>İzmir ve Bilkent seminerleri</div>
      </div>
      <div class="mg-decade">
        <div class="mg-decade-label">2000</div>
        <div class="mg-tl-event"><strong>2000</strong>Osmanlı İmparatorluğu'nda Devlet ve Ekonomi kitabı</div>
        <div class="mg-tl-event"><strong>2006</strong>Osmanlı Maliyesi Kurumlar ve Bütçeler</div>
        <div class="mg-tl-event"><strong>2009</strong>TRT belgeseli: Tarihin Işığında Bir Ömür</div>
      </div>
      <div class="mg-decade">
        <div class="mg-decade-label">2010</div>
        <div class="mg-tl-event"><strong>2011</strong>Altunizade konferans serisi (6 bölüm)</div>
        <div class="mg-tl-event"><strong>2013</strong>Dört Sima Armağan kitabı yayını</div>
        <div class="mg-tl-event"><strong>2015</strong>TÜBA Şeref Ödülü</div>
        <div class="mg-tl-event"><strong>2018</strong>Şehir Üniversitesi son dersleri</div>
      </div>
      <div class="mg-decade">
        <div class="mg-decade-label">2020</div>
        <div class="mg-tl-event"><strong>2021</strong>Osmanlı Ekonomisine Dair Konuşmalar I</div>
        <div class="mg-tl-event"><strong>2021</strong>Vefat · 18 Mart</div>
        <div class="mg-tl-event"><strong>2022</strong>Hac Yolunda Bir Karınca biyografisi</div>
        <div class="mg-tl-event"><strong>2023</strong>Anısına uluslararası sempozyum</div>
      </div>
    </div>

    <div class="mg-tl-footer">
      <p>Tüm kronoloji için zaman çizelgesini ziyaret edin.</p>
      <a href="https://hacyolundabirkarinca.github.io/mgenc/timeline.html" class="btn-outline-gold">Tam Kronoloji →</a>
    </div>
  </div>
</section>

<!-- ════════ PORTAL KAPILAR ════════ -->
<section class="mg-section mg-portals">
  <div class="mg-section-inner">
    <div class="mg-section-label">Koleksiyon</div>
    <h2 class="mg-section-title">Nereden Başlamak İstersiniz?</h2>
    <p class="mg-section-sub">Koleksiyonu üç ana kapıdan keşfedebilirsiniz.</p>
    <div class="mg-portal-grid">

      <a href="https://hacyolundabirkarinca.github.io/mgenc/browse.html" class="mg-portal-card">
        <div class="mg-portal-icon">📚</div>
        <div class="mg-portal-name">Akademik Üretim</div>
        <p class="mg-portal-desc">Konferans bildirileri, makaleler, kitap bölümleri ve söyleşiler. Yarım asrın entelektüel birikimi.</p>
        <div class="mg-portal-tags">
          <span class="mg-portal-tag">Konferans & Bildiri</span>
          <span class="mg-portal-tag">Yazılı Eserler</span>
          <span class="mg-portal-tag">Röportaj & Söyleşi</span>
        </div>
        <div class="mg-portal-count"><span>229 kayıt</span><span class="mg-portal-arrow">→</span></div>
      </a>

      <a href="https://hacyolundabirkarinca.github.io/mgenc/browse.html" class="mg-portal-card">
        <div class="mg-portal-icon">🖼️</div>
        <div class="mg-portal-name">Görsel Arşiv</div>
        <p class="mg-portal-desc">Fotoğraflar ve video kayıtları. Çalıştaylar, dersler, söyleşiler ve özel anlar.</p>
        <div class="mg-portal-tags">
          <span class="mg-portal-tag">Fotoğraflar</span>
          <span class="mg-portal-tag">Video Kayıtları</span>
        </div>
        <div class="mg-portal-count"><span>114 kayıt</span><span class="mg-portal-arrow">→</span></div>
      </a>

      <a href="https://hacyolundabirkarinca.github.io/mgenc/browse.html" class="mg-portal-card">
        <div class="mg-portal-icon">👤</div>
        <div class="mg-portal-name">Biyografik</div>
        <p class="mg-portal-desc">Aile arşivi, hayat hikâyesi, vefeyat yazıları ve anma metinleri.</p>
        <div class="mg-portal-tags">
          <span class="mg-portal-tag">Aile Arşivi</span>
          <span class="mg-portal-tag">Hayat Hikâyesi</span>
          <span class="mg-portal-tag">Vefeyat & Anma</span>
        </div>
        <div class="mg-portal-count"><span>88 kayıt</span><span class="mg-portal-arrow">→</span></div>
      </a>

    </div>
  </div>

  <div class="mg-section-inner" style="margin-top:3rem;padding-top:3rem;border-top:1px solid var(--border)">
    <div class="mg-section-label">Koleksiyon Özeti</div>
    <h2 class="mg-section-title">442 Kayıt, Bir Ömür</h2>
    <div class="mg-data-grid">
      <a href="https://hacyolundabirkarinca.github.io/mgenc/browse.html" class="mg-data-card">
        <div class="mg-data-icon">📄</div>
        <div class="mg-data-num">122</div>
        <div class="mg-data-label">PDF / Belge</div>
      </a>
      <a href="https://hacyolundabirkarinca.github.io/mgenc/browse.html" class="mg-data-card">
        <div class="mg-data-icon">🖼</div>
        <div class="mg-data-num">267</div>
        <div class="mg-data-label">Fotoğraf & Görsel</div>
      </a>
      <a href="https://hacyolundabirkarinca.github.io/mgenc/browse.html" class="mg-data-card">
        <div class="mg-data-icon">▶</div>
        <div class="mg-data-num">53</div>
        <div class="mg-data-label">Video</div>
      </a>
      <a href="https://hacyolundabirkarinca.github.io/mgenc/map.html" class="mg-data-card">
        <div class="mg-data-icon">🗺</div>
        <div class="mg-data-num">40+</div>
        <div class="mg-data-label">Şehir & Ülke</div>
      </a>
    </div>
  </div>
</section><!-- ════════ KONULAR ════════ -->
<section class="mg-section mg-topics">
  <div class="mg-section-inner">
    <div class="mg-section-label">Konular</div>
    <h2 class="mg-section-title">Öne Çıkan Temalar</h2>
    <p class="mg-section-sub">Koleksiyonda en sık karşılaşılan kavramlar ve izlekler.</p>
    <div class="mg-topic-cloud">
      <a href="https://hacyolundabirkarinca.github.io/mgenc/subjects.html" class="mg-topic-tag large">İktisat</a>
      <a href="https://hacyolundabirkarinca.github.io/mgenc/subjects.html" class="mg-topic-tag large">Konferans</a>
      <a href="https://hacyolundabirkarinca.github.io/mgenc/subjects.html" class="mg-topic-tag medium">Tarihçilik</a>
      <a href="https://hacyolundabirkarinca.github.io/mgenc/subjects.html" class="mg-topic-tag medium">Devlet</a>
      <a href="https://hacyolundabirkarinca.github.io/mgenc/subjects.html" class="mg-topic-tag medium">Ticaret</a>
      <a href="https://hacyolundabirkarinca.github.io/mgenc/subjects.html" class="mg-topic-tag medium">18. Yüzyıl</a>
      <a href="https://hacyolundabirkarinca.github.io/mgenc/subjects.html" class="mg-topic-tag medium">Maliye</a>
      <a href="https://hacyolundabirkarinca.github.io/mgenc/subjects.html" class="mg-topic-tag small">Biyografi</a>
      <a href="https://hacyolundabirkarinca.github.io/mgenc/subjects.html" class="mg-topic-tag small">Vergi</a>
      <a href="https://hacyolundabirkarinca.github.io/mgenc/subjects.html" class="mg-topic-tag small">İktisadi Düşünce</a>
      <a href="https://hacyolundabirkarinca.github.io/mgenc/subjects.html" class="mg-topic-tag small">Vakıflar</a>
      <a href="https://hacyolundabirkarinca.github.io/mgenc/subjects.html" class="mg-topic-tag small">Arşiv</a>
      <a href="https://hacyolundabirkarinca.github.io/mgenc/subjects.html" class="mg-topic-tag small">19. Yüzyıl</a>
      <a href="https://hacyolundabirkarinca.github.io/mgenc/subjects.html" class="mg-topic-tag small">Kişiler</a>
      <a href="https://hacyolundabirkarinca.github.io/mgenc/subjects.html" class="mg-topic-tag small">Sanayii</a>
    </div>
  </div>
</section>


</div><!-- #mg-home -->
<script>
(function(){
  var tl = document.getElementById('mgTimeline');
  if(tl){
    tl.addEventListener('wheel', function(e){
      if(Math.abs(e.deltaY) > Math.abs(e.deltaX)){
        e.preventDefault();
        tl.scrollLeft += e.deltaY;
      }
    }, { passive: false });
  }
})();
</script>
