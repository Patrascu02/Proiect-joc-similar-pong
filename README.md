NUME PROIECT:

Joc Interactiv Pong cu Paddle și Mingii

INTRODUCERE: 

Prezentarea pe scurt a proiectului:
Proiectul implementează un joc interactiv bazat pe un joystick, o matrice LED 8x8, un ecran LCD și două butoane. Scopul jocului este să controlezi un paddle pentru a lansa o minge către o țintă poziționată (o alta minge)aleator pe matricea LED.

CE FACE ?

Controlează paddle-ul utilizând un joystick.
Simulează mișcarea mingii 2, care poate fi reflectată de paddle, pereți sau margini.
Gestionează coliziunile și pierderile de vieți.
Afișează scorul, nivelul, timpul de joc și viețile pe un ecran LCD.
Emite sunete pentru evenimente precum coliziuni și pierderea vieților.
Permite pauzarea jocului pe un buton și oprirea lui si pornirea lui  cu ajutorul celuilalt buton.
Care este scopul lui:
Scopul proiectului este de a oferi o experiență interactivă, îmbinând elemente de hardware și software, pentru a simula un joc captivant.

IDEEA DE LA CARE AM PORNIT :

Am dorit să implementăm un joc clasic de tip Pong cu funcționalități moderne și să demonstrăm utilizarea practică a mai multor module hardware și software.

DE CE ESTE UTIL :

-Pentru utilizatori: Este un joc educativ și distractiv.

-Pentru noi: Ne dezvoltă abilitățile de programare, proiectare hardware și integrare a componentelor.

DESCRIERE GENERALA :

-Schematica bloc:

-->Joystick: Controlează mișcarea paddle-ului sus/jos pe matricea LED.
-->Matrice LED 8x8: Afișează paddle-ul, mingea 2 și mingea 1 (ținta).
-->Ecran LCD: Afișează informații despre scor, nivel, vieți și timp.

-Butoane:

1)Start joc si Oprire
2) Pauza

-Sunet: Indică diverse evenimente prin beep-uri.
-Microcontroler (ATmega): Coordonează toate funcțiile jocului.
-Alimentare: Sursă de 5V pentru toate componentele.

HARDWARE DESIGN:
 
-Listă de componente:

Microcontroler: ATmega328P.
Joystick analogic.
Matrice LED 8x8 cu driver MAX7219.
Ecran LCD 16x2 cu I2C.
Butoane tactile x2.
Rezistențe: Diverse valori pentru conexiuni.
Buzzer.
Surse de alimentare: 5V (baterie sau adaptor).
Fire, breadboard sau PCB.
Schematica electrică:
(Va fi realizată într-o aplicație precum KiCAD sau Tinkercad, specificând conexiunile între microcontroler și periferice.)

SOFTWARE DESIGN:

Mediu de dezvoltare:
PlatformIO.
Biblioteci folosite:
Adafruit_GFX și Adafruit_LED_Backpack pentru matricea LED.
LiquidCrystal_I2C pentru ecranul LCD.
TimerOne pentru generarea de sunete.
Algoritmi și structuri:
State machine: Gestionează stările jocului (start, pauză, joc activ, game over).
Mișcare mingii:
Vectori de direcție pentru mingea 2.
Algoritm pentru coliziuni (cu paddle, margini, pereți).
Scor și nivel:
Creștere scor și afișare pe LCD.
Accelerare mingii la fiecare 10 puncte.
Funcții principale:
setup(): Inițializări hardware și software.
loop(): Logica principală a jocului.
Mișcarea mingii: Gestionarea poziției și coliziunilor.
Control paddle: Actualizarea poziției paddle-ului pe baza joystick-ului.
Update LCD: Afișare scor, nivel, vieți și timp.
Gestionare butoane: Start, pauză și oprire.
Rezultate Obținute
Paddle-ul este controlat precis de joystick.
Mingea interacționează corect cu paddle-ul, peretele și marginea.
Afișarea pe LCD funcționează corespunzător.
Sunetele sunt redate în momentele potrivite.
Concluzii
Proiectul a demonstrat integrarea cu succes a componentelor hardware și software pentru un joc funcțional. Am învățat despre utilizarea joystick-urilor, a matricelor LED și a tehnicilor de optimizare a codului pentru microcontrolere.

Cod sursă și alte resurse:

Codul sursă este organizat în directorul src.
Schemele hardware sunt în directorul hardware.
Fotografii și videoclipuri cu proiectul sunt în directorul images.

Bibliografie/Resurse:
-Hardware:
    -->Datasheet-uri pentru ATmega328P, MAX7219, LCD.
-Software:
    -->Documentație biblioteci PlatformIO.
    -->Tutoriale pentru joystick-uri și matrice LED.
