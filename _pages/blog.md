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
🇺🇸 USA, 🇲🇽 Mexico, 🇯🇵 Japan, 🇳🇱 Netherlands, 🇫🇷 France, 🇪🇸 Spain, 🇨🇳 China,
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

  function makePin(color) {
    return L.divIcon({
      html: '<i class="fa-solid fa-location-dot" style="color:' + color + '; font-size:1.2rem; filter:drop-shadow(0 1px 2px rgba(0,0,0,0.12));"></i>',
      iconSize: [20, 20], iconAnchor: [10, 20], tooltipAnchor: [0, -16], className: ''
    });
  }
  var mint = makePin("#44cfba");
  var pink = makePin("#ffb6c1");
  var lavender = makePin("#d0bfff");

  // Lived (pink)
  var lived = [
    ["Yeosu, South Korea", 34.74, 127.66], ["Jeonju, South Korea", 35.82, 127.15],
    ["Pohang, South Korea", 36.02, 129.37], ["Ulsan, South Korea", 35.54, 129.31],
    ["Daejeon, South Korea", 36.35, 127.38], ["Seoul, South Korea", 37.57, 126.98],
    ["Seosan, South Korea", 36.78, 126.45],
    ["Atlanta, GA", 33.75, -84.39]
  ];

  // Nature / National Parks (lavender)
  var nature = [
    ["Yosemite, CA", 37.75, -119.59], ["Big Sur, CA", 36.27, -121.81],
    ["Zion, UT", 37.30, -113.03], ["Bryce Canyon, UT", 37.59, -112.19],
    ["Grand Canyon, AZ", 36.11, -112.11], ["Antelope Canyon, AZ", 36.86, -111.37],
    ["Horseshoe Bend, AZ", 36.88, -111.51], ["Everglades, FL", 25.75, -80.94],
    ["Huangshan, China", 30.13, 118.17], ["Mount Rigi, Switzerland", 47.06, 8.48],
    ["Jeju Island, South Korea", 33.49, 126.53]
  ];

  // Visited (mint) - everything else
  var visited = [
    ["San Francisco, CA", 37.77, -122.42], ["Berkeley, CA", 37.87, -122.27],
    ["Sausalito, CA", 37.86, -122.49], ["Tiburon, CA", 37.87, -122.46],
    ["Palo Alto, CA", 37.44, -122.14], ["Napa, CA", 38.30, -122.30],
    ["Los Angeles, CA", 34.05, -118.24],
    ["Las Vegas, NV", 36.17, -115.14],
    ["Houston, TX", 29.76, -95.37], ["Austin, TX", 30.27, -97.74],
    ["Boston, MA", 42.36, -71.06], ["New York, NY", 40.71, -74.01],
    ["Washington, DC", 38.91, -77.04], ["Chattanooga, TN", 35.05, -85.31],
    ["Athens, GA", 33.96, -83.38],
    ["Panama City Beach, FL", 30.18, -85.80], ["Rosemary Beach, FL", 30.28, -86.01],
    ["Miami, FL", 25.76, -80.19], ["Fort Lauderdale, FL", 26.12, -80.14],
    ["Chicago, IL", 41.88, -87.63], ["Urbana-Champaign, IL", 40.11, -88.21],
    ["Cancun, Mexico", 21.16, -86.85],
    ["Tokyo, Japan", 35.68, 139.69], ["Osaka, Japan", 34.69, 135.50], ["Kyoto, Japan", 35.01, 135.77],
    ["Amsterdam, Netherlands", 52.37, 4.90], ["Haarlem, Netherlands", 52.38, 4.64], ["Utrecht, Netherlands", 52.09, 5.12],
    ["The Hague, Netherlands", 52.08, 4.30], ["Delft, Netherlands", 52.01, 4.36], ["Alkmaar, Netherlands", 52.63, 4.75],
    ["Zaanse Schans, Netherlands", 52.47, 4.77],
    ["Paris, France", 48.86, 2.35],
    ["Madrid, Spain", 40.42, -3.70], ["Barcelona, Spain", 41.39, 2.17],
    ["Granada, Spain", 37.18, -3.60], ["Seville, Spain", 37.39, -5.98],
    ["Shanghai, China", 31.23, 121.47],
    ["Kota Kinabalu, Malaysia", 5.98, 116.07],
    ["Sydney, Australia", -33.87, 151.21],
    ["Budapest, Hungary", 47.50, 19.04],
    ["Prague, Czech Republic", 50.08, 14.44],
    ["Vienna, Austria", 48.21, 16.37], ["Salzburg, Austria", 47.81, 13.05],
    ["Berlin, Germany", 52.52, 13.41], ["Munich, Germany", 48.14, 11.58],
    ["Dresden, Germany", 51.05, 13.74],
    ["Bratislava, Slovakia", 48.15, 17.11]
  ];

  var livedLayer = L.layerGroup();
  var visitedLayer = L.layerGroup();
  var natureLayer = L.layerGroup();

  visited.forEach(function (c) { L.marker([c[1], c[2]], { icon: mint }).bindTooltip(c[0], { direction: "top" }).addTo(visitedLayer); });
  lived.forEach(function (c) { L.marker([c[1], c[2]], { icon: pink }).bindTooltip(c[0], { direction: "top" }).addTo(livedLayer); });
  nature.forEach(function (c) { L.marker([c[1], c[2]], { icon: lavender }).bindTooltip(c[0], { direction: "top" }).addTo(natureLayer); });

  livedLayer.addTo(map);
  visitedLayer.addTo(map);
  natureLayer.addTo(map);

  // Legend with toggle
  var legend = L.control({ position: "bottomright" });
  legend.onAdd = function () {
    var div = L.DomUtil.create("div", "legend");
    div.style.cssText = "background:white; padding:8px 12px; border-radius:8px; box-shadow:0 1px 4px rgba(0,0,0,0.2); font-size:0.75rem; line-height:2; cursor:pointer; user-select:none;";
    var items = [
      { color: "#ffb6c1", label: "Lived", layer: livedLayer },
      { color: "#44cfba", label: "Visited", layer: visitedLayer },
      { color: "#d0bfff", label: "Nature", layer: natureLayer }
    ];
    items.forEach(function (item) {
      var row = L.DomUtil.create("div", "", div);
      row.innerHTML = '<i class="fa-solid fa-location-dot" style="color:' + item.color + ';"></i> ' + item.label;
      row.style.cssText = "transition: opacity 0.2s;";
      row.addEventListener("click", function (e) {
        L.DomEvent.stopPropagation(e);
        if (map.hasLayer(item.layer)) {
          map.removeLayer(item.layer);
          row.style.opacity = "0.35";
        } else {
          map.addLayer(item.layer);
          row.style.opacity = "1";
        }
      });
    });
    return div;
  };
  legend.addTo(map);
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

In the **KBO**, I root for the **Kia Tigers** 🐯 — my hometown team that I've supported since childhood.

In the **MLB**, living in Atlanta made it natural to become a **Braves** fan.
I love the unique vibe and style of the Atlanta Braves — especially the Tomahawk Chop! 🪓

</div>
</div>

---

## 🎵 Amateur Oboist & Classical Music Enthusiast

I am an amateur oboist and a devoted classical music enthusiast.
I have experience playing oboe in several leading halls in Europe (e.g. Musikverein),
and won a gold medal at the Honam Arts Festival at age 13.

#### 🎬 Last Performance in Korea (Feb. 2024)

The encore from nearly my last performance before moving to the US.
An unforgettable and precious memory -
performing with my favorite people in my favorite ensemble.

<div style="max-width: 360px; aspect-ratio: 9/16;">
<iframe width="100%" height="100%" src="https://www.youtube.com/embed/JQYK1McKo9o" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe>
</div>

<br>

#### 🎶 Instruments

<span style="font-size: 1.4rem;">𝄞</span> **Oboe / English Horn** (from 2007, high level, active amateur guest player)

🎻 **Viola** (from 2018, intermediate)

#### 💜 Favorite Pieces

🎼 **Symphonies**: Dvorak No. 9 (2nd mvt), Sibelius No. 2, Mahler No. 3 (6th mvt), Mahler No. 6 (2nd mvt), R. Strauss *Eine Alpensinfonie*, Tchaikovsky No. 6 (1st mvt), Holst *The Planets*

🎹 **Concertos**: Beethoven "Emperor" (2nd mvt), Chopin Piano Concerto No. 1 & 2 (2nd mvt)

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
