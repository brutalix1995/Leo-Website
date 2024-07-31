---
title: "UmbauBunker"
weight: 2
cover:
    image: "UmbauBunker-transparent.png"
cover.hiddenInSingle: true
hideSummary: true
hidefooter: false
ShowBreadCrumbs: true
---

{{< rawhtml >}}
<!DOCTYPE html>
<html>
  <head>
    <title>Slideshow Images</title>
    <style>
      * {
        box-sizing: border-box
      }
      body {
        margin: 0
      }
      .mySlides {
        display: none
      }
      img {
        vertical-align: middle;
      }
      .slideshow-container {
        max-width: 1000px;
        position: relative;
        margin: auto;
      }
      /* Next & previous buttons */
      .prev {
        cursor: pointer;
        position: absolute;
        top: 50%;
        width: 6%;
        padding: 10px;
        margin-top: -22px;
        color: transparent;
        transition: 0.6s ease;
        border-radius: 30px;
        user-select: none;
        left: -10%;
      }
      .next {
        cursor: pointer;
        position: absolute;
        top: 50%;
        width: 6%;
        padding: 10px;
        margin-top: -22px;
        color: transparent;
        transition: 0.6s ease;
        border-radius: 30px;
        user-select: none;
        right: -10%; /* Position the "next button" to the right */
      }
      /* On hover, add a black background color with a little bit see-through */
      .prev:hover,
      .next:hover {
        background-color: rgba(108, 108, 108, 0.5);
      }
      /* Caption text */
      .text {
        color: #ffffff;
        font-size: 15px;
        padding: 8px 12px;
        position: absolute;
        bottom: 8px;
        width: 100%;
        text-align: center;
      }
      /* Number text (1/3 etc) */
      .numbertext {
        color: #ffffff;
        font-size: 12px;
        padding: 8px 12px;
        position: absolute;
        top: 0;
      }
      /* The dots/bullets/indicators */
      .dot {
        cursor: pointer;
        height: 15px;
        width: 15px;
        margin: 0 2px;
        background-color: #999999;
        border-radius: 50%;
        display: inline-block;
        transition: background-color 0.6s ease;
      }
      .active,
      .dot:hover {
        background-color: #111111;
      }
      /* Fading animation */
      .fade {
        -webkit-animation-name: slide;
        -webkit-animation-duration: 1.5s;
        animation-name: slide;
        animation-duration: 1.5s;
      }
      @-webkit-keyframes fade {
        from {
          opacity: .4
        }
        to {
          opacity: 1
        }
      }
      @keyframes fade {
        from {
          opacity: .4
        }
        to {
          opacity: 1
        }
      }
      /* On smaller screens, decrease text size */
      @media only screen and (max-width: 840px) {
        .prev { 
          left: 2%;
          width: 10%;
          }
        .next { 
          right: 2%;
          width: 10%;
          }
        .text {
          font-size: 11px
        }
      }
    </style>
  </head>
  <body>
    <div class="slideshow-container">
      <div class="mySlides fade">
        <img src="/UmbauBunker2.jpg" style="width:100%">
      </div>
      <div class="mySlides fade">
        <img src="/UmbauBunker3.jpg" style="width:100%">
      </div>
      <div class="mySlides fade">
        <img src="/UmbauBunker4.jpg" style="width:100%">
      </div>
      <div class="mySlides fade">
        <img src="/UmbauBunker5.jpg" style="width:100%">
      </div>
      <div class="mySlides fade">
        <img src="/UmbauBunker6.jpg" style="width:100%">
      </div>
      <div class="mySlides fade">
        <img src="/UmbauBunker7.jpg" style="width:100%">
      </div>
       <div class="mySlides fade">
        <img src="/UmbauBunker8.jpg" style="width:100%">
      </div>
      <div class="mySlides fade">
        <img src="/UmbauBunker9.jpg" style="width:100%">
      </div>
      <a class="prev" onclick="plusSlides(-1)"><img src="/Pfeil-Links.png"></a>
      <a class="next" onclick="plusSlides(1)"><img src="/Pfeil-Rechts.png"></a>
    </div>
    <br>
    <div style="text-align:center">
      <span class="dot" onclick="currentSlide(0)"></span>
      <span class="dot" onclick="currentSlide(1)"></span>
      <span class="dot" onclick="currentSlide(2)"></span>
      <span class="dot" onclick="currentSlide(4)"></span>
      <span class="dot" onclick="currentSlide(5)"></span>
      <span class="dot" onclick="currentSlide(6)"></span>
      <span class="dot" onclick="currentSlide(7)"></span>
      <span class="dot" onclick="currentSlide(8)"></span>
    </div>
    <script>
      let slideIndex = 0;
      let timeoutId = null;
      const slides = document.getElementsByClassName("mySlides");
      const dots = document.getElementsByClassName("dot");
      showSlides();
      function currentSlide(index) {
           slideIndex = index;
           showSlides();
      }
     function plusSlides(step) {
         if(step < 0) {
            slideIndex -= 2;
            if(slideIndex < 0) {
              slideIndex = slides.length - 1;
            }
        }
        showSlides();
     }
      function showSlides() {
        for(let i = 0; i < slides.length; i++) {
          slides[i].style.display = "none";
          dots[i].classList.remove('active');
        }
        slideIndex++;
        if(slideIndex > slides.length) {
          slideIndex = 1
        }
        slides[slideIndex - 1].style.display = "block";
        dots[slideIndex - 1].classList.add('active');
         if(timeoutId) {
            clearTimeout(timeoutId);
         }
        timeoutId = setTimeout(showSlides, 5000); // Change image every 5 seconds
      }
    </script>
  </body>
</html>
{{< /rawhtml >}}

### ENTWURF

Von Außen her wirkt der
Bunker wie ein hermetisch
abgeriegelter Quader. Mittlerweile wurde das alte
Walmdach abgetragen und
zeigt den wuchtigen Dachstuhl aus Stahlbeton. Kleine in die Fassade einge-
lassene Luftlöcher sind
die einzigen Elemente, die
sonst vollkommen geschlossene Fassade öffnen. Durch
jeweils sechs Eingänge kann
der Bunker betreten werden.
Sein Grundriss ist symmetrisch gegliedert und lässt
sich in zwei Achsen aufteilen.

### KONZEPT

Basis des Entwurfs ist das
Box in Box-Prinzip. Wir
planen die Betonhülle des
Bunkers aufzubrechen und
diese als thermische Hülle
zu benutzen. Da der Bunker in seiner Grundsubstanz
sehr großzügige Raumhöhen
aufweist, planen wir die
zweite Decke ab beginn des
Erdgeschosses zu entfernen.
Die dadurch gewonnene neue
Raumhöhe machen wir uns zu
Nutzen.
In die einzelnen Geschosse
werden neue Holzeinbauten
mittels Ständerwerk eingebaut. Die Kisten als solches werden gedämmt. Zur
Nutzung des Bauwerkes werden Öffnungen in der Fassade
hergestellt. Um ausreichend
Raumhöhe gewährleisten zu
können müssen mindestens
drei Decken aufgebrochen
werden. Je Geschoss werden
zwei Wohneinheiten ausgewiesen. Diese sind um die
115 m² groß.

### Konstruktion

Die Fassade wird durch ein
Öffnungsraster aufgelockert,
welches aus schmalen hochrechteckigen und quadratischen Öffnungen besteht. Die
Öffnungen springen im Versatz und bringen so eine
Dynamik in die Fassade. Die
Öffnungen an den Ecken des
Bunkers bilden nach hinten
Loggien aus. Die Deckendurchbrüche in der Nordseite werden bildnach innen geöffnet, sodass sich
ein Hof öffnet. Dieser wird
durch ein Peristyl ergänzt,
welches eine bepflanzte Mitte mit einem umlaufenden
Gang aufweist. Ein dreigeschossiger Aufbau in Holzbauweise wird auf die obere
1,40 m starke Schutzdecke
gestellt.
Dieser übernimmt im seine Raumorganisation für den
oberen Teil des Bunkers.
Das zentrale Treppenhaus
wird umgeplant und bis
in den Holzaufbau weitergeführt. zusätzlich wird
ein Aufzug eingeplant. Zum
Flachdach hin, welches begrünt werden kann öffnet
sich über dem Treppenhaus
eine Laterne, welche den
Tageslichteinfall ins Treppenhaus ermöglicht und den
Zugang aufs Dach bietet.

Mit der Wiedernutzbarmachung des weitgehend leer
stehenden Bunkers soll dieser einer neuen und sinnvollen Nutzung zugeführt
werden. Einen Abriss halten
wir aufgrund seiner Bausubstanz für unverhältnismäßig. Diese Thesen werden
wir im folgenden Bericht
umfangreich erläutern.