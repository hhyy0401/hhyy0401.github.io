---
layout: page
permalink: /life/
title: life
nav: true
nav_order: 5
description:
---

## 🏃‍♀️ Running & 🏊‍♀️ Swimming & 🚴‍♀️ Cycling

<div class="row mt-3">
<div class="col-sm-4 mt-3 mt-md-0">
{% include figure.liquid loading="eager" path="assets/img/running.jpeg" class="img-fluid rounded z-depth-1" zoomable=true %}
</div>
<div class="col-sm-8 mt-3 mt-md-0" markdown="1">

I'm passionate about endurance sports - running, swimming, and cycling.
My half marathon personal best is **2:04:22**.

One of my favorite places on campus is the **Georgia Tech Aquatic Center** -
home of the 1996 Atlanta Olympic swimming events, featuring a 50m-length, 3m-depth pool.
It's where I love to swim laps between research sessions!

Growing up in Yeosu, a beautiful coastal city in southern Korea, I loved cycling along the seaside roads as a child.

</div>
</div>

---

## ✈️ Travelling

<div class="row mt-3">
<div class="col-sm-8 mt-3 mt-md-0" markdown="1">

I love travelling and exploring new cultures, food, and landscapes.
So far I've visited **16 countries** across 4 continents.
I enjoy the vast nature and the unique culture and history of each country.

**Countries visited** (most recent first):
🇺🇸 USA, 🇲🇽 Mexico (Cancun), 🇯🇵 Japan, 🇳🇱 Netherlands, 🇫🇷 France, 🇪🇸 Spain, 🇨🇳 China (Shanghai),
🇲🇾 Malaysia, 🇦🇺 Australia, 🇭🇺 Hungary, 🇨🇿 Czech Republic, 🇦🇹 Austria, 🇩🇪 Germany, 🇨🇭 Switzerland, 🇸🇰 Slovakia, 🇰🇷 South Korea.

</div>
<div class="col-sm-4 mt-3 mt-md-0">
{% include figure.liquid loading="eager" path="assets/img/travel.png" class="img-fluid rounded z-depth-1" style="max-width: 220px;" zoomable=true %}
</div>
</div>

<div id="travel-map" style="width: 100%; height: 420px; border-radius: 12px; overflow: hidden; margin: 0.5rem 0;"></div>

<link rel="stylesheet" href="https://cdn.jsdelivr.net/npm/leaflet@1.9.4/dist/leaflet.min.css" />
<script src="https://cdn.jsdelivr.net/npm/leaflet@1.9.4/dist/leaflet.min.js"></script>

<script>
document.addEventListener("DOMContentLoaded", function () {
  var map = L.map("travel-map", { scrollWheelZoom: false }).setView([25, 20], 2);
  L.tileLayer("https://{s}.basemaps.cartocdn.com/rastertiles/voyager/{z}/{x}/{y}{r}.png", {
    attribution: '&copy; <a href="https://carto.com/">CARTO</a>',
    maxZoom: 18
  }).addTo(map);

  var pin = L.icon({
    iconUrl: "https://cdn.jsdelivr.net/npm/leaflet@1.9.4/dist/images/marker-icon.png",
    iconRetinaUrl: "https://cdn.jsdelivr.net/npm/leaflet@1.9.4/dist/images/marker-icon-2x.png",
    shadowUrl: "https://cdn.jsdelivr.net/npm/leaflet@1.9.4/dist/images/marker-shadow.png",
    iconSize: [25, 41], iconAnchor: [12, 41], popupAnchor: [1, -34], shadowSize: [41, 41]
  });

  [
    ["USA", 37.09, -95.71], ["Mexico (Cancun)", 21.16, -86.85], ["Japan", 36.20, 138.25],
    ["Netherlands", 52.13, 5.29], ["France", 46.23, 2.21], ["Spain", 40.46, -3.75],
    ["China (Shanghai)", 31.23, 121.47], ["Malaysia", 4.21, 101.98], ["Australia", -25.27, 133.78],
    ["Hungary", 47.16, 19.50], ["Czech Republic", 49.82, 15.47], ["Austria", 47.52, 14.55],
    ["Germany", 51.17, 10.45], ["Switzerland", 46.82, 8.23], ["Slovakia", 48.67, 19.70],
    ["South Korea", 35.91, 127.77]
  ].forEach(function (c) {
    L.marker([c[1], c[2]], { icon: pin }).addTo(map).bindPopup("<b>" + c[0] + "</b>");
  });
});
</script>

---

## ⚾ Baseball

<div class="row mt-3">
<div class="col-sm-4 mt-3 mt-md-0">
{% include figure.liquid loading="eager" path="assets/img/baseball.jpeg" class="img-fluid rounded z-depth-1" zoomable=true %}
</div>
<div class="col-sm-8 mt-3 mt-md-0" markdown="1">

I'm a passionate baseball fan who follows both Korean and American baseball.

In the **KBO**, I root for the **Kia Tigers** - my hometown team that I've supported since childhood.

In the **MLB**, living in Atlanta made it natural to become a **Braves** fan.
I love the unique vibe and style of the Atlanta Braves — especially the Tomahawk Chop!

</div>
</div>

---

## 🎵 Amateur Oboist & Classical Music Enthusiast

I am an amateur oboist and a devoted classical music enthusiast.
I have experience playing oboe in several leading halls in Europe (e.g. Musikverein),
and won a gold medal at the Honam Arts Festival at age 13.

### 🎬 Last Performance in Korea (Feb. 2024)

The encore from nearly my last performance before moving to the US.
An unforgettable and precious memory -
performing with my favorite people in my favorite ensemble.

<div style="max-width: 360px; aspect-ratio: 9/16;">
<iframe width="100%" height="100%" src="https://www.youtube.com/embed/JQYK1McKo9o" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe>
</div>

### 🎶 Instruments

- **Oboe / English Horn** (from 2007, high level, active amateur guest player)
- **Viola** (from 2018, intermediate)

### 💜 Favorite Pieces

**Symphonies**: Dvorak No. 9 (2nd mvt), Sibelius No. 2, Mahler No. 3 (6th mvt), Mahler No. 6 (2nd mvt), R. Strauss *Eine Alpensinfonie*, Tchaikovsky No. 6 (1st mvt), Holst *The Planets*

**Concertos**: Beethoven "Emperor" (2nd mvt), Chopin Piano Concerto No. 1 & 2 (2nd mvt)

<details>
<summary><strong>Performance History: 2011 European Tour (1st Oboe)</strong></summary>
<div markdown="1">

| Ensemble | Repertoire | Venue |
|---|---|---|
| Yeodo Elementary School Orchestra | Rienzi Overture, Zigeunerweisen, Dvorak No. 9, Ruslan and Ludmilla | Slovak Radio Hall, World Trade Center Patria Hall, Lukaskirche, Rudolfinum Dvorak Hall, Musikverein, Mozarteum Grosser Saal |

</div>
</details>

<details>
<summary><strong>Performance History: 2012-2014 Middle School (1st Oboe)</strong></summary>
<div markdown="1">

| Ensemble | Repertoire | Venue |
|---|---|---|
| Yeosu Young Talent Orchestra | Light Cavalry Overture, Poet and Peasant | Yeosu Yeulmaru |
| Yeodo Elementary + Middle School | Nabucco Overture, Schubert No. 8 | Seongnam Art Center |
| Yeosu Young Talent Orchestra | Poet and Peasant, Finlandia | Yeosu Yeulmaru |
| Yeodo Middle School | Radetzky March, Carmen Overture, Gabriel's Oboe (solo concerto) | Yeosu Marine Park |

</div>
</details>

<details>
<summary><strong>Performance History: 2018-2021 University (POSTECH)</strong></summary>
<div markdown="1">

| Ensemble | Repertoire | Part |
|---|---|---|
| POSTECH Orchestra | Waltz of the Flowers | Ob1 |
| POSTECH Orchestra | Rosamunde Overture, Haydn "Farewell" 4th mvt, Tchaikovsky No. 5 | Ob1 |
| POSTECH Orchestra | Beethoven No. 7, Schubert No. 5 | Ob1 |
| HanUlRim | Waltz of the Flowers, Rach Piano Concerto No. 2 (arr.) | Viola |
| HanUlRim | Spring Waltz, Clair de Lune, Pomp and Circumstance, Rietz Oboe Concerto 1st mvt (solo) | Ob1, Viola |
| *Ulsan Opus One | Saint-Saens Bacchanale | Ob1 |
| *Handong University | Egmont Overture, Schubert No. 8 | Ob1 |
| AOU "Shall we dance?" | Nutcracker Suite, Rachmaninoff Symphonic Dances, Danzon No. 2 | Ob1 |
| HanUlRim | Gliere Horn Concerto 2nd mvt, Chronicles of Narnia | Conductor |

</div>
</details>

<details>
<summary><strong>Performance History: 2022- After Moving to Seoul (* = guest player)</strong></summary>
<div markdown="1">

| Ensemble | Repertoire | Part | Venue |
|---|---|---|---|
| *Univ. of Seoul Cantabile | Holst Planets No. 4 Jupiter, Bruch Violin Concerto, Tchaikovsky No. 5 | Ob2 | Goyang Aramnuri |
| *Sogang Univ. ACES | Nutcracker Suite, Slave March, Danse Macabre | Eng.H, Ob2 | Gangbuk Arts Center |
| AOU MONOMYTH | Borodin Prince Igor, Dvorak Hero's Song, Borodin No. 2 | Viola | Seongnam Art Center |
| HUFS Hufsphil | Sibelius Violin Concerto, Sibelius No. 2 | Ob1 | Goyang Aramnuri |
| Apoco | Mahler No. 5 | Eng.H, Ob3 | Seongnam Art Center |
| *HanUlRim | Haydn No. 100, Danzon No. 2, Schubert Cello Concerto 3rd mvt, Pictures at an Exhibition (parts) | Eng.H, Ob | POSTECH Auditorium |
| *Dongguk Univ. OPUS | Midsummer Night's Dream (parts), Krommer Clarinet Concerto 1st mvt, Beethoven No. 6 (Ob1) | Ob1, Ob2 | Sowol Art Hall |
| *Sogang Univ. ACES | Marriage of Figaro Overture, Swan Lake, Chaminade Flute Concerto, Zigeunerweisen, Finlandia, Dvorak No. 9 (2nd mvt: Ob2+Eng.H) | Eng.H, Ob1 | Chugye Univ. Concert Hall |
| Chung-Ang Univ. Rubato | Tchaikovsky Romeo and Juliet, Tchaikovsky Violin Concerto, Tchaikovsky No. 6 | Ob1 | Mapo Art Center |
| *Kwangwoon Univ. DaKAPO | Suppe Poet and Peasant, Nutcracker Suite (parts), Rachmaninoff No. 2 (Ob1) | Ob1, Ob2 | Seongnam Atrium |
| *Smile Healing Forte | Beethoven "Emperor", Brahms No. 2 | Ob2 | Gwacheon Civic Center |
| *Sookmyung Pharmacy SPHO | Suppe Poet and Peasant, Blue Danube, Beethoven No. 5 (Ob1) | Ob1, Ob2 | Bucheon Civic Center |
| *Sungkyunkwan Univ. SKKUO | Beethoven Ruins of Athens Overture, Reinecke Flute Concerto, Beethoven No. 7 | Ob2 | Anyang Art Center |
| Apoco | Ravel La Valse, Prokofiev No. 5 | Ob1 | Seongnam Art Center |
| Sogang Univ. ACES | Sibelius Finlandia (choir), Tchaikovsky 1812 (choir), Beethoven No. 9 (choir) | Ob1 | Chugye Univ. Concert Hall |
| CHAOS | Ravel Pavane, Prokofiev No. 1, Mozart No. 41 "Jupiter", Marriage of Figaro, Holst Jupiter (excerpt) | Ob1 | Bukseoul Dream Forest Art Center |
| *KUMO | Beethoven Egmont Overture, Grieg Peer Gynt Suite (excerpt), Beethoven No. 7 | Ob2 | Gwanglim Art Center |
| *HUFS Hufsphil | Brahms Tragic Overture, Mendelssohn Violin Concerto, Tchaikovsky No. 5 | Ob2 | Seoul Art Center Doam Hall |
| *Ewha Womans Univ. ESAOS | Grieg Peer Gynt Suite (excerpt), Smetana Moldau, Tchaikovsky No. 6 | Ob1 | Ewha Auditorium |
| KAMPh | Shostakovich Festive Overture, Tchaikovsky Fate Overture, Shostakovich No. 5, Wagner Lohengrin Act 3 Prelude | Ob1 | Icheon Art Center |
| AOU Finale | Carmen Suite No. 1 (Eng.H), Mahler No. 1 | Eng.H, Ob3 | Bucheon Art Center |
| CHAOS | Debussy Clair de Lune (arr.), Borodin String Quartet Nocturne (arr.), Debussy Petite Suite, Beethoven No. 2, Elgar Salut d'Amour (arr.), Spirited Away | Eng.H, Ob1, Ob2 | Bukseoul Dream Forest Art Center |
| *Ewha Womans Univ. ESAOS | Brahms Piano Concerto No. 1, Brahms No. 1 | Ob1 | Ewha Auditorium |

</div>
</details>

For my full music profile, visit my [Notion page](https://hyunju-music.notion.site/Hyunju-s-Music-Profile-7dfe265521ac4470842a21739ce5ff18).
