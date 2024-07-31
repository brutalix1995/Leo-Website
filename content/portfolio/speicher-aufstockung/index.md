---
title: "Aufstockung"
weight: 3
cover:
    image: "Aufstockung-transparent.png"
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
        <img src="/Aufstockung2.jpg" style="width:100%">
      </div>
      <div class="mySlides fade">
        <img src="/Aufstockung3.jpg" style="width:100%">
      </div>
      <div class="mySlides fade">
        <img src="/Aufstockung4.jpg" style="width:100%">
      </div>
      <div class="mySlides fade">
        <img src="/Aufstockung5.jpg" style="width:100%">
      </div>
      <div class="mySlides fade">
        <img src="/Aufstockung6.jpg" style="width:100%">
      </div>
      <div class="mySlides fade">
        <img src="/Aufstockung7.jpg" style="width:100%">
      </div>
       <div class="mySlides fade">
        <img src="/Aufstockung8.jpg" style="width:100%">
      </div>
      <div class="mySlides fade">
        <img src="/Aufstockung10.jpg" style="width:100%">
      </div>
      <div class="mySlides fade">
        <img src="/Aufstockung9.jpg" style="width:100%">
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
      <span class="dot" onclick="currentSlide(9)"></span>
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

### KONZEPT

Das Gebäude in der Speditionsstraße 15A verdeutlicht in seiner Struktur
noch seinen Ursprung als
Lager- und Logistikgebäude im Hafen. Heute dient
es als Keimzelle für innovative Start-ups und trägt
so zum lebendigen Mix von
Architekturen und Nutzungen
im Düsseldorfer Medienhafen
bei.
Angesichts der robusten
Tragstruktur des Gebäudes
liegt es nahe, durch nachhaltige Flächenaktivierung
einen attraktiven Gewerbestandort zu schaffen. Die
Vorgaben des Brandschutzes
erlauben jedoch nur eine
zusätzliche Etage unterhalb
von 22 Metern über Straßenniveau.
Die Aufstockung setzt diese
Vorgaben in einem modernen
städtebaulichen Prototypen um. Die Erweiterung ist
als nahezu autarke Infrastruktur konzipiert, die
mit minimalen Eingriffen die
bestehende Gebäudestruktur
respektiert und das Ensemble durch ein charakteristisches Alleinstellungsmerkmal als neue “Krone”.

### Materialität

Die Einfügung in den Gesamtkontext des Hafenensembles entlang der Speditionsstraße bestimmt die
Materialwahl der Gebäudehülle. Die Bekleidung aus
Cortenstahl fügt sich harmonisch in den Bestand und
die umliegenden Ziegelbauten ein und reflektiert den
industriellen Ursprung des
Ortes. Die metallische Hülle der Aufstockung verleiht
dem Gebäude einen präzisen,
scharfkantigen Charakter
und ermöglicht gleichzeitig
die geschwungene Wellenform.
Die Konstruktion besteht
aus vorgefertigten Massivholzteilen, wodurch die Erweiterung in kürzester Zeit
auf den Bestand montiert
werden kann. Dies minimiert den Bedarf an Baustelleneinrichtungen, was
den Gegebenheiten vor Ort
entgegenkommt. Das Projekt bleibt vollständig
demontierbar und nachhaltig. Neben den funktionalen
Aspekten entsteht so eine
Bürofläche mit hohem emotionalen Wert und optimalem
Arbeitsklima.

### Idee

Der Entwurf leitet sich
aus dem strengen Raster
des funktionalen Bestandsgebäudes ab und verfolgt
das Ziel, die Erweiterung
modular und leicht industriell wirken zu lassen.
Dieser Baukörper übernimmt
die Struktur und Abmessungen des Bestands, löst sich
jedoch leicht schwebend von
der bestehenden Dachhaut
ab und betont seine Eigenständigkeit. Konstruktion,
Ausbau und Fassade können
einfach maschinell vorgefertigt und wirtschaftlich
errichtet werden.
Nach außen zeigt der Entwurf seine Individualität.
Die um fünf Meter in den
Luftraum geschobene Fassadenbox eröffnet den Blick
auf das Wasser und zur Altstadt. Die obere Kante der
Fassade schwingt in einer
unverwechselbaren Wellenform und betont die Besonderheit des Ortes. Zusätzliche Photovoltaikelemente
sorgen für eine nahezu autarke Energieversorgung.

### Nutzungen

Zentrales Element des
Grundrisses ist eine großzügige Treppe, die die
Büro- und Showroomfläche mit
der Dachterrasse verbindet. Diese zweite Ebene der
Aufstockung bietet vielfältige Nutzungsmöglichkeiten
unter freiem Himmel: Arbeiten, Entspannen, Feiern.
Die Wellenform des Dachaufbaus setzt die Bewegung
der Treppe nach außen hin
sichtbar fort.
