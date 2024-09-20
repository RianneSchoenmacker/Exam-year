## Sensorintegratie

## Hoe kan ik het kleed laten activeren?

### 1. Gewichtssensoren / Druksensoren
- **Drukgevoelige Pads**: Gebruik druksensoren die het licht aanzetten wanneer er druk op wordt uitgeoefend. Dit kan een andere manier zijn om interactie te detecteren en het licht te activeren.
- **Integratie**: Deze sensor kan in je werkstuk worden geïntegreerd om gebieden te detecteren waar druk wordt uitgeoefend en vervolgens de verlichting te regelen.  
  Deze sensoren kunnen detecteren hoeveel gewicht er op een bepaald gebied van het kleed wordt geplaatst. Ze kunnen nuttig zijn om het licht in te schakelen wanneer iemand op het kleed staat of drukt.

- **Load Cell**:
  - *Wat is het?*: Load cells meten fysieke kracht, meestal druk of gewicht, en zetten deze om in elektrische signalen.
  - *Gebruik*: Je kunt ze onder het kleed plaatsen om het gewicht van iemand te detecteren. In combinatie met een versterker (bijv. HX711) kunnen ze zelfs lichte druk meten.
  - *Aanbevolen voor*: Het detecteren van gewicht of druk op specifieke plekken in het kleed.

- [Kapton + Copper Matrix](https://www.kobakant.at/DIY/?p=7443)

### 2. Touchsensoren
- **Capacitive Touch Sensors**: Gebruik capacitive touch sensors om het licht in te schakelen wanneer iemand het werkstuk aanraakt. Deze sensors detecteren veranderingen in elektrische capaciteit veroorzaakt door aanraking en kunnen worden aangesloten op een microcontroller die de LEDs aanstuurt.
- **Instellingen en Aanpassingen**: Zorg ervoor dat de sensors correct zijn afgesteld en gevoelig genoeg zijn om te reageren op aanraking zonder ongewenste valse triggers.

- **Capacitieve Touchsensor (bijv. TTP223)**:
  - *Wat is het?*: Deze sensoren meten veranderingen in capacitieve lading wanneer ze worden aangeraakt. Ze reageren op lichte aanraking en kunnen discreet onder de stof van het kleed worden geplaatst.
  - *Gebruik*: Geschikt voor het detecteren van aanrakingen op de oppervlakte van het kleed. Ze zijn eenvoudig te gebruiken en kunnen makkelijk geïntegreerd worden in een interactief lichtsysteem.
  - *Aanbevolen voor*: Licht activeren door aanraking of beweging op het kleed.

- **Force Sensitive Resistor (FSR)**:
  - *Wat is het?*: Dit is een druksensor die weerstand meet afhankelijk van de druk die erop wordt uitgeoefend. Hoe harder de druk, hoe lager de weerstand.
  - *Gebruik*: Plaats ze onder het kleed of in de tuftlagen om zachte druk of aanrakingen te meten. Ze reageren goed op zowel druk als aanraking.
  - *Aanbevolen voor*: Licht activeren door druk of aanraking, met de mogelijkheid om de intensiteit van het licht aan te passen op basis van de druk.

- [Force Sensitive Resistor uitleg](https://www.youtube.com/watch?v=qjruYfwsOaI)  
  (Kan dit achter het hele kleed?)

### 3. Afstandssensoren
- **Bewegingssensoren**: Gebruik een bewegingssensor zoals een PIR-sensor (Passieve Infraroodsensor) om licht te activeren op basis van beweging in de buurt van je werkstuk.
- **Instelbare Sensitiviteit**: Zorg ervoor dat de sensitiviteit van de bewegingssensor kan worden aangepast om alleen te reageren op relevante bewegingen.

- **Ultrasone Afstandssensor (HC-SR04)**:
  - *Wat is het?*: Een ultrasone sensor die geluidsgolven gebruikt om de afstand tot een object te meten. Het is een betrouwbare en goedkope sensor voor korte afstanden.
  - *Gebruik*: Deze sensoren kunnen worden gebruikt om de afstand te meten en het licht in te schakelen wanneer iemand het kleed nadert. Plaats ze bij de randen of onder het kleed.
  - *Aanbevolen voor*: Automatisch activeren van licht wanneer iemand het kleed benadert.

- **IR Afstandssensor (bijv. Sharp GP2Y0A02YK0F)**:
  - *Wat is het?*: Een infrarood afstandssensor die infrarood licht gebruikt om de afstand te meten. Hij werkt goed op korte tot middellange afstanden en is iets nauwkeuriger dan ultrasone sensoren.
  - *Gebruik*: Deze kan ook aan de rand van het kleed worden geplaatst om beweging te detecteren wanneer iemand in de buurt komt.
  - *Aanbevolen voor*: Bewegingsdetectie van personen in de buurt van het kleed.

- **Kinect**:
  - *Wat is het?*: Een camera die kan worden gebruikt om beweging en personen te detecteren.
  - *Aanbevolen voor*: Bewegingsdetectie van personen voor het kleed, of als je een soort 'spiegel' wilt maken.

### 4. Knop of Schakelaar
- **Handmatige Controle**: Voor een eenvoudigere benadering kun je een knop of schakelaar integreren in je werkstuk die het licht in- en uitschakelt. Dit kan een fysieke knop zijn die de verlichting regelt.
  - *Extra idee*: Je kunt er een spel van maken waarbij je de schakelaars in het kleed moet vinden.

### 5. Microcontroller en Programmatie
- **Arduino of andere Microcontrollers**: Als je een microcontroller zoals een Arduino gebruikt, kun je deze programmeren om de verschillende sensoren te lezen en op basis van die input de LEDs aan te sturen. Dit biedt veel flexibiliteit en controle over hoe en wanneer het licht aan en uit gaat.
- **Code Voorbeeld**: Je kunt een eenvoudige code schrijven die de sensorwaarden leest en op basis van die waarden de LEDs in- of uitschakelt. Er zijn veel voorbeelden en bibliotheken beschikbaar die je kunnen helpen met dit soort projecten.



## Kapton + Copper Matrix

Ik wil beginnen met het maken van de:
- [Kapton + Copper Matrix](https://www.kobakant.at/DIY/?p=7443)

Ik denk dat ik hiermee de beste resultaten kan halen. Ik heb de producten besteld en ga hier mee testen veel producten zoals de geleidende verf heb ik nog nooit mee gewerkt dus zal ik ook beginnende experimenten mee doen om te kijken hoe het werkt en hoe het reageert.

Wat ik heirvoor nodig/besteld en hoe ik getest heb:

- Kapton-tape: Dit is een dunne, flexibele, hittebestendige tape die vaak wordt gebruikt in elektronica. Het dient als de isolator in de matrix.

- Kopertape of woven geleidende tape: Een zelfklevende tape gemaakt van koper of gelijdende draad, die als geleidende laag dient in je sensor.

<div style="display: flex; justify-content: space-between;">
    <img src="../images/sensoren/kopertape.jpg" alt="Afbeelding 1" width="200"/>
    <img src="../images/sensoren/kopertapecircuit.jpg" alt="Afbeelding 2" width="200"/>
    <img src="../images/sensoren/kopertapecircuitaan.jpg" alt="Afbeelding 3" width="200"/>
</div>

<div style="display: flex; justify-content: space-between;">
    <img src="../images/sensoren/woventape.jpg" alt="Afbeelding 1" width="200"/>
    <img src="../images/sensoren/woventapecircuit.jpg" alt="Afbeelding 2" width="200"/>
    <img src="../images/sensoren/woventapecircuitaan.jpg" alt="Afbeelding 3" width="200"/>
</div>

- Elektrische geleidende verf: Als alternatief voor kopertape kun je geleidende verf gebruiken om patronen te schilderen op de Kapton-tape.

<div style="display: flex; justify-content: space-between;">
    <img src="../images/sensoren/geleidendverf.jpg" alt="Afbeelding 1" width="200"/>
    <img src="../images/sensoren/geleidendverfcircuit.jpg" alt="Afbeelding 2" width="200"/>
    <img src="../images/sensoren/geleidendverfcircuitaan.jpg" alt="Afbeelding 3" width="200"/>
</div>

- Solderen of geleidend lijm: Dit is nodig om de kopertape met de rest van je circuit te verbinden.

- Draden of kabels: Om de kopertape of geleidende verf aan te sluiten op de elektronische componenten (zoals een microcontroller).

- Microcontroller (bijv. Arduino of ESP): Deze is nodig om de signalen van de matrixsensor te verwerken en verdere acties (zoals het activeren van verlichting) aan te sturen.

Ik ben begonnen met de koper tape de Matrix te maken op karton. Ik heb de coper tape beverstigd en daaraan draden gesoldeerd. Vervolgens heb ik getest of het de stroom nog wel geleid door dit te meten.

<div style="display: flex; justify-content: space-between;">
    <img src="../images/sensoren/druksensormaken1.jpg" alt="Afbeelding 1" width="200"/>
    <img src="../images/sensoren/druksensormaken2.jpg" alt="Afbeelding 1" width="200"/>
    <img src="../images/sensoren/druksensormaken3.jpg" alt="Afbeelding 3" width="200"/>
</div>

<div style="display: flex; justify-content: space-between;">
    <img src="../images/sensoren/druksensormaken4.jpg" alt="Afbeelding 1" width="200"/>
    <img src="../images/sensoren/druksensormaken5.jpg" alt="Afbeelding 1" width="200"/>
</div>

Helaas werkt mijn code nog niet dus ben er nog druk mee bezig maar het is wel gelukt een soort meting te maken. 

<div style="display: flex; justify-content: space-between;">
    <img src="../images/sensoren/Matrixtest.png" alt="Afbeelding 1" width="200"/>
</div>
