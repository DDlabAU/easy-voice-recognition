# --- **WORK IN PROGRESS** ---
# EasyVR tutorial

## Hvad er EasyVR?

EasyVR er et 'Arduino shield', der lader dig koble en mikrofon og højttaler på en Arduino og derefter bruge stemmegenkendelse til at styre Arduinoen med.

Denne tutorial hjælper dig med at få easyVR op at køre og styre enkel elektronik. Derfra kan du selv arbejde videre med dit konkrete projekt og eventuelt forbinde dit projekt med internettet eller lignende.


## Krav

- Windows (skal bruges for at programmere EasyVR-modulet. Du kan komme i DD Lab og bruge en Windowsmaskine, hvis du ikke har selv).
- Arduinomiljøet


## Software

### Voice Commander
#### Installation

Der er en række forskellig software du skal have på plads, for at du kan bruge EasyVR:

- Manual og software. Download fra: <http://www.veear.eu/downloads/>
- Installér først software på din computer (kun Windows)
- Installér derefter Arduinobiblioteket fra Arduinomiljøet (gå til Sketch → Include Library → Manage Libraries → søg efter EasyVR → Install).
- Advarsel: Hvis du henter via SparkFun får du et ældre library (på det tidspunkt vi lavede guiden)

#### Hul igennem

Før du går videre med træning skal du sikre at der er hul igennem til Arduinoen og EasyVR-modulet. Åbn derfor Arduinomiljøet, når du har installeret software fra pkt. 1.

Vælg File → Examples → EasyVR → TestEasyVR og upload den store mængde kode til Arduinoen, som normalt. Dette er koden der ligger på Arduinoen (i modsætning til EasyVR-'shieldet', der indeholder lydklip, )

#### Stemmetræning og Commander-softwaren

Du bruger Commander-softwaren til at træne EasyVR-modulet og til at generere koden, der senere skal uploades gennem Arduinomiljøet.
Du kan i princippet skrive al koden direkte i Arduinomiljøet, men det er uden for scope af denne tutorial.

Det er ikke svært at kode de forskellige nøgleord ind gennem Commander-softwaren, men det kan være lidt svært at gennemskue, så derfor har vi lavet en video, der kan ses her:

___VIDEO HER___

#### Bemærk
Du skal indstille dig på at prøve forskellig afstande til mikrofonen, både i forhold til at indspille og registrere nøgleordene du vælger. For mere information angående mikrofonen kan du læse fra side 11 i manualen.

### Arduinokode


## Hardware

### Opsætning
EasyVR-modulet består af flere dele: et shield, selve EasyVR-boardet, en mikrofon og en lille højtaler.

EasyVR-modulet består af flere dele:
- Et shield
- Selve EasyVR-boardet
- En mikrofon
- En lille højtaler

Et arduino shield er et board man sætter oven på sin arduino for at udvide dens funktionalitet. Shields bygges så de passer på et bestemt type board. I dette tilfælde er EasyVR-shieldet bygget til at passe på en arduino UNO eller boards med samme størrelse og layout, f.eks. sparkfun redboards.
Det smarte ved shields er, at vi slipper for selv at skulle forbinde en komponent med vores arduino, som vi plejer at gøre gennem et breadboard eller ved at lodde dem direkte sammen. De er også utroligt nemme at bruge, da shieldet bare skal sættes ovenpå arduinoen og kun kan side på én måde. Det er altså næsten umuligt at gøre forkert.

I dette tilfælde er shieldet to-delt og det er faktisk muligt at tage komponenten af, hvis du skulle have lyst til at anvende modulet med et andet board. Det er dog en anelse mere komplekst og uden for scope af denne tutorial.
