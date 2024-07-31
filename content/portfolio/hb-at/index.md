---
title: "HB-AT"
weight: 4
cover:
    image: "HB_Turm-transparent.png"
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
        <img src="/HB_Turm2.jpg" style="width:100%">
      </div>
      <div class="mySlides fade">
        <img src="/HB_Turm3.jpg" style="width:100%">
      </div>
      <div class="mySlides fade">
        <img src="/HB_Turm4.jpg" style="width:100%">
      </div>
      <div class="mySlides fade">
        <img src="/HB_Turm5.jpg" style="width:100%">
      </div>
      <div class="mySlides fade">
        <img src="/HB_Turm6.jpg" style="width:100%">
      </div>
      <div class="mySlides fade">
        <img src="/HB_Turm7.jpg" style="width:100%">
      </div>
       <div class="mySlides fade">
        <img src="/HB_Turm8.jpg" style="width:100%">
      </div>
      <div class="mySlides fade">
        <img src="/HB_Turm9.jpg" style="width:100%">
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

### Konzept

Der HB AT, der neue Aussichtsturm für den Hülser Berg in Krefeld, soll Besuchern eine umfassende Aussichtserfahrung bieten und gleichzeitig als markantes Bauwerk in der Landschaft fungieren. Der Entwurf kombiniert moderne Architektur mit funktionalen Aspekten, um sowohl ästhetische als auch praktische Anforderungen zu erfüllen.

### Struktur und Materialien

Der Turm ist in Stahlgerüstbauweise ausgeführt und mit lichtdurchlässigen PVC-Platten verkleidet. Für das Gerüst wird recycelter Stahl verwendet, um die Umweltbelastung zu minimieren und Ressourcen zu schonen. Diese Kombination gewährleistet eine hohe Stabilität und Langlebigkeit des Bauwerks. Die PVC-Platten lassen Tageslicht durch und schaffen eine helle, angenehme Atmosphäre im Inneren des Turms.

### Idee

Der des HB AT umfasst mehrere Ebenen, die durch eine spiralförmige Treppenkonstruktion verbunden sind. Die organischen, geschwungenen Formen der Treppen und Plattformen fügen sich harmonisch in die natürliche Umgebung ein. Die geschwungenen Treppen und Plattformen erinnern an natürliche Strukturen wie Kletterpflanzen, was die Verbindung zwischen Architektur und Natur betont und den Besuchern ein einzigartiges visuelles Erlebnis bietet.

### Funktionen und Nutzung

- Aussichtsplattform: Die oberste Plattform bietet einen weiten Blick über die Landschaft und ist überdacht, um Schutz vor Witterungseinflüssen zu bieten. 
- Treppen: Die spiralförmige Treppenkonstruktion ermöglicht einen bequemen Aufstieg. Stabile Geländer sorgen für Sicherheit. 
- Eingang: Der Eingang ist durch eine markante Struktur gekennzeichnet, die den Zugang erleichtert und den Übergang zur ersten Treppe nahtlos gestaltet.

### Nachhaltigkeit

Der Turm ist so konzipiert, dass er umweltfreundlich ist. Die Verwendung von recyceltem Stahl und die Integration in die natürliche Umgebung reduzieren den ökologischen Fußabdruck. Solarmodule auf dem Dach der Aussichtsplattform könnten den Turm mit nachhaltiger Energie versorgen.

Der Turm vereint modernes Design mit funktionaler Architektur und einer nachhaltigen Bauweise. Er dient als Attraktion für Besucher und fügt sich harmonisch in die Landschaft ein.