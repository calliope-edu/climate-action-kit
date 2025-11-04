# Mobile Irrigation System - Use Tutorial

```package
fwd-climate-action=github:Forward-Education/pxt-climate-action#v1.1.0
datalogger=datalogger
v3
```

```template
fwdButtons.touch1.onEvent(jacdac.ButtonEvent.Down, function () {
    for (let index = 0; index < 4; index++) {
        fwdMotors.drive(fwdEnums.ForwardReverse.Forward, 25)
        basic.pause(3000)
        fwdMotors.stop()
        fwdLights.ledRing1.setAllPixelsColor(0x00ff00)
        fwdMotors.pump.timedRun(1500)
        basic.pause(3000)
        fwdLights.ledRing1.setAllPixelsColor(0xff0000)
    }
})
fwdMotors.setupDriving(
fwdBase.rightServo,
fwdBase.leftServo,
45
)
fwdLights.ledRing1.setAllPixelsColor(0xff0000)
```

## Aktivität 1: Erstelle dein Projekt @showdialog

Lasst uns ein mobiles Bewässerungssystem bauen! Wir werden dies in drei Schritten tun:

1. **Bauen:** Dein Fahrzeug
2. **Code erstellen:** Um dein Fahrzeuug zum Leben zu erwecken
3. **Ausprobieren:** Teste dein Fahrzeug, um zu erfahren, wie es funktioniert


<img src="https://raw.githubusercontent.com/calliope-edu/climate-action-kit/main/tutorial-assets/hs-mobileirrigation-render.webp" alt="Full mobile irrigation render" style="display: block; width: 60%; margin:auto;">

## Bauanleitung Schritt 1 @showdialog

![sbs1](https://raw.githubusercontent.com/calliope-edu/climate-action-kit/main/tutorial-assets/hs-mobileirrigation-sbs01.webp)

## Bauanleitung Schritt 2 @showdialog

![sbs1](https://raw.githubusercontent.com/calliope-edu/climate-action-kit/main/tutorial-assets/hs-mobileirrigation-sbs02.webp)

## Bauanleitung Schritt 3 @showdialog

![sbs1](https://raw.githubusercontent.com/calliope-edu/climate-action-kit/main/tutorial-assets/hs-mobileirrigation-sbs03.webp)

## Bauanleitung Schritt 4 @showdialog

![sbs1](https://raw.githubusercontent.com/calliope-edu/climate-action-kit/main/tutorial-assets/hs-mobileirrigation-sbs04.webp)

## Bauanleitung Schritt 5 @showdialog

![sbs1](https://raw.githubusercontent.com/calliope-edu/climate-action-kit/main/tutorial-assets/hs-mobileirrigation-sbs05.webp)

## Bauanleitung Schritt 6 @showdialog

![sbs1](https://raw.githubusercontent.com/calliope-edu/climate-action-kit/main/tutorial-assets/hs-mobileirrigation-sbs06.webp)

## Bauanleitung Schritt 7 @showdialog

![sbs1](https://raw.githubusercontent.com/calliope-edu/climate-action-kit/main/tutorial-assets/hs-mobileirrigation-sbs07.webp)

## Bauanleitung Schritt 8 @showdialog

![sbs1](https://raw.githubusercontent.com/calliope-edu/climate-action-kit/main/tutorial-assets/hs-mobileirrigation-sbs08.webp)

## Bauanleitung Schritt 9 @showdialog

![sbs1](https://raw.githubusercontent.com/calliope-edu/climate-action-kit/main/tutorial-assets/hs-mobileirrigation-sbs09.webp)

## Bauanleitung Schritt 10 @showdialog

![sbs1](https://raw.githubusercontent.com/calliope-edu/climate-action-kit/main/tutorial-assets/hs-mobileirrigation-sbs10.webp)

## Bauanleitung Schritt 11 @showdialog

![sbs1](https://raw.githubusercontent.com/calliope-edu/climate-action-kit/main/tutorial-assets/hs-mobileirrigation-sbs11.webp)

## Bauanleitung Schritt 12 @showdialog

![sbs1](https://raw.githubusercontent.com/calliope-edu/climate-action-kit/main/tutorial-assets/hs-mobileirrigation-sbs12.webp)

## Bauanleitung Schritt 13 @showdialog

![sbs1](https://raw.githubusercontent.com/calliope-edu/climate-action-kit/main/tutorial-assets/hs-mobileirrigation-sbs13.webp)

## Bauanleitung Schritt 14 @showdialog

![sbs1](https://raw.githubusercontent.com/calliope-edu/climate-action-kit/main/tutorial-assets/hs-mobileirrigation-sbs14.webp)

## Bauanleitung Schritt 15 @showdialog

![sbs1](https://raw.githubusercontent.com/calliope-edu/climate-action-kit/main/tutorial-assets/hs-mobileirrigation-sbs15.webp)

Hinweis: Setze die Pumpe einfach auf das Fahrzeug. Während der Erprobung des Prototyps wird kein Wasser verwendet.

## Bauanleitung Schritt 16 @showdialog

![sbs1](https://raw.githubusercontent.com/calliope-edu/climate-action-kit/main/tutorial-assets/hs-mobileirrigation-sbs16.webp)

## Bauanleitung Schritt 17 @showdialog

![sbs1](https://raw.githubusercontent.com/calliope-edu/climate-action-kit/main/tutorial-assets/hs-mobileirrigation-sbs17.webp)

Hinweis: Wenn du den Kunststoffschlauch an der Pumpe befestigen möchtest, kannst du ihn um diesen mittleren Rahmen herum befestigen und durch die Servoöffnung führen. Dadurch wird sichergestellt, dass das Wasser aus dem hinteren Teil des Fahrzeugs kommt.

## Bauanleitung Schritt 18 @showdialog

![sbs1](https://raw.githubusercontent.com/calliope-edu/climate-action-kit/main/tutorial-assets/hs-mobileirrigation-sbs18.webp)

## Bauanleitung Schritt 19 @showdialog

![sbs1](https://raw.githubusercontent.com/calliope-edu/climate-action-kit/main/tutorial-assets/hs-mobileirrigation-sbs19.webp)

## Bauanleitung Schritt 20 @showdialog

![sbs1](https://raw.githubusercontent.com/calliope-edu/climate-action-kit/main/tutorial-assets/hs-mobileirrigation-sbs20.webp)

## Activity 2: Code Your Project @showdialog

Wir müssen unser Modell mit dem Computer verbinden, damit es mit Code zum Leben erweckt werden kann!

Der Code enthält die Anweisungen, die unserem Calliope mini sagen, was er tun soll.

## Code Step 1 @showdialog

WICHTIG! Vergewissere dich, dass dein Climate Action Kit Breakout Board eingeschaltet und dein Calliope mini an einem Computer angeschlossen ist.

<img src="https://raw.githubusercontent.com/calliope-edu/climate-action-kit/main/tutorial-assets/pluganim.webp" alt="Plug Calliope mini into USB port on computer" style="display: block; width: 40%; margin:auto;">

## Code Step 2 @showdialog

Klicke auf die drei Punkte neben der Schaltfläche `|Download|` und dann auf „Gerät verbinden“.
Befolge anschließend die Schritte zum Koppeln des Calliope mini.

<img src="https://raw.githubusercontent.com/calliope-edu/climate-action-kit/main/tutorial-assets/pairmicrobitGIF.webp"  alt="Pairing gif" style="display: block; width: 60%; margin:auto;">

## Code Step 3

Klicke anschließend auf die Schaltfläche `|Download|`, um den Code vom Projekt herunterzuladen.

## Activity 3: Use Your Project @showdialog

Wir sind nun bereit, unser mobiles Bewässerungssystem zu **verwenden**!

**Tipps zum Tutorial**

- **Verwende** die Anweisungen oben auf dem Bildschirm.
- Wenn du weitere Informationen benötigst, klicke auf **„Mehr erfahren!“** ().
- Wenn du Hilfe beim Code benötigst, klicke auf die **Glühbirne**!

<img src="https://raw.githubusercontent.com/calliope-edu/climate-action-kit/main/tutorial-assets/tellmore_hintbox_gif.webp" style="display: block; width: 80%; margin:auto;">

## Ausprobieren Schritt 1

Schaue dir das mobile Bewässerungssystem, das du gerade gebaut hast, genau an. Kannst jedes verwendete Teil identifizieren und benennen?
~hint Mehr erfahren!
Dieses System verwendet:

-   **Bausteine:** Die Grundplatte, vier lange Rahmen mit Servo-Bohrungen, vier mittelgroße Rahmen, einen mittelgroßen Rahmen mit Servo-Bohrungen, drei dünne Rahmen, vier kleine Rahmen, vier Würfelverbinder, acht Eckverbinder und zwei Räder
-   **Roboterteile:** Eine Breakout-Platine, Calliope mini, zwei stufenlose Servomotoren, einen LED-Ring, einen Berührungssensor und einen Sonarsensor
    hint~

## Ausprobieren Schritt 2

Wie funktionieren deiner Meinung nach all diese Teile zusammen, damit das Fahrzeug fährt?
~hint Mehr erfahren!
- Die Bausteine bilden eine Struktur, die einer Vielzahl von Kräften standhalten kann.
- Der Calliope mini erfasst die **Eingaben** des Benutzers über den Berührungssensor.
- Der Calliope mini kommuniziert mit der Pumpe, den Motoren und dem LED-Ring und teilt jedem mit, wann er aktiviert werden soll. Diese Komponenten liefern unsere **Ausgabe**.
- Alle Teile müssen über die Breakout-Platine und Kabel korrekt verbunden und programmiert sein, um einen reibungslosen Betrieb zu gewährleisten.
    hint~

## Ausprobieren Schritt 3

Schaue dir den unten angegebenen Code an.

Was wird deiner Meinung nach passieren, wenn du das Programm ausführst? Welche Teile des Codes haben deine Vorhersage beeinflusst?
## Ausprobieren Schritt 4

Starte das Fahrzeug durch Drücken des Berührungssensors. Beobachte, was passiert.

Hat sich das Fahrzeug so verhalten, wie du es vorhergesagt hast? Wenn nicht, was war anders? Kannst du diese Unterschiede erklären?

~hint Mehr erfahren!
Wenn der Berührungssensor aktiviert wird, führt das Fahrzeug folgende Schritte aus:

1. Es fährt 3 Sekunden lang vorwärts.
2. Es hält an.
3. Es schaltet die grünen LEDs ein, um anzuzeigen, dass die Bewässerung beginnt.
4. Es lässt die Pumpe 1,5 Sekunden lang laufen, um die Pflanzen zu bewässern.
5. Es schaltet die roten LEDs ein, um anzuzeigen, dass die Bewässerung abgeschlossen ist.

Dieser Vorgang wiederholt sich viermal.
hint~

```blocks
fwdButtons.touch1.onEvent(jacdac.ButtonEvent.Down, function () {
    for (let index = 0; index < 4; index++) {
        fwdMotors.drive(fwdEnums.ForwardReverse.Forward, 25)
        basic.pause(3000)
        fwdMotors.stop()
        fwdLights.ledRing1.setAllPixelsColor(0x00ff00)
        fwdMotors.pump.timedRun(1500)
        basic.pause(3000)
        fwdLights.ledRing1.setAllPixelsColor(0xff0000)
    }
})
```

## Ausprobieren Schritt 5

Fahre das Fahrzeug erneut. Berechne diesmal die Geschwindigkeit deines mobilen Bewässerungsfahrzeugs.

Die Kenntnis der Geschwindigkeit hilft uns zu verstehen, wie effizient das Fahrzeug arbeitet.
~hint Mehr erfahren!

-   **So geht's:** Versuche es mit[this worksheet](https://docs.google.com/spreadsheets/d/1lbxG2hC1mEXjtbOMv5Cthnl1_vBMQ_CALTbgO4zxMbk/edit?gid=0#gid=0). Messe die zurückgelegte Strecke deines Fahrzeugs. Messe die Zeit, die dein Fahrzeug benötigt, um diese Strecke zurückzulegen.
-   **Steigung:** Wenn du mehrere Datenpunkte entlang der Fahrtstrecke deines Fahrzeugs grafisch darstellen, sollte die Steigung der besten Passgeraden die Geschwindigkeit des Fahrzeugs darstellen. Verwende diese Formel: **Geschwindigkeit = Entfernung / Zeit**
-   **Analysieren Sie Ihre Ergebnisse:** Wie schnell fährt dein Fahrzeug? Welche Faktoren beeinflussen seine Geschwindigkeit?
    hint~

## Wassereinsparungsmodellierung @showdialog

Lassen Sie uns anhand der Geschwindigkeit einige Berechnungen durchführen, um zu ermitteln, wie viel Wasser dieses System einsparen kann.

## Modellierungsschritt 1

Überlegen Sie zunächst, wie viel Wasser verbraucht würde, wenn die Pumpe bei einem Hub von 100 cm _kontinuierlich_ laufen würde.

_Hinweis: Nehmen Sie an, dass die maximale Durchflussrate der Pumpe etwa 28 ml/Sekunde beträgt._
~hint Mehr erfahren!
Die Gleichung zur Berechnung des Wasserverbrauchs für ein kontinuierliches System lautet: 𝑊(d) = 𝑟 × (d/𝑣)
Bedeutet:

-   𝑊(d) ist der Gesamtwasserverbrauch in Millilitern
-   𝑟 ist die Pumpengeschwindigkeit in Millilitern pro Sekunde (28 ml/Sekunde)
-   d ist die Gesamtstrecke, die das Fahrzeug in Zentimetern zurücklegt
-   𝑣 ist die Geschwindigkeit des Fahrzeugs in Zentimetern pro Sekunde
    hint~

## Modellierungsschritt Schritt 2

Glücklicherweise läuft die Pumpe in dem von uns gerade gebauten Prototyp nur in regelmäßigen Abständen. Wie viel Wasser würde dieser Prototyp bei einer Fahrt von 100 cm verbrauchen? Welche Gleichung würdest du in diesem Szenario verwenden?

Überlege, welche Variablen du berücksichtigen musst (z. B. Zeit, Entfernung, Fahrzeuggeschwindigkeit, Pumpendrehzahl/Durchflussrate, Pumpzeit usw.). In welchem Zusammenhang stehen diese Variablen mit dem Wasserverbrauch im aktuellen Prototyp?

~hint Mehr erfahren!
Um den Wasserverbrauch für das gerade gebaute mobile Bewässerungssystem zu berechnen, verwenden wir folgende Gleichung: 𝑊(d) = 𝑟 × d × fd × tp
Bedeutet:

- 𝑊(d) ist der Wasserverbrauch in Millilitern
- 𝑟 ist die Pumpgeschwindigkeit in Millilitern pro Sekunde (28 ml/Sekunde)
- fd ist die Pumpfrequenz (z. B. Anzahl der Aktivierungen pro Zentimeter)
- d ist die zurückgelegte Gesamtstrecke in cm
- tp ist die Pumpzeit pro Aktivierung (1,5 Sekunden)
    hint~

## Modellierungsschritt Schritt 3

Schließlich ist es an der Zeit zu berechnen, wie viel Wasser dieser Prototyp im Vergleich zum kontinuierlichen System einspart.

Ziehe den Wasserverbrauch des Prototyps vom Wasserverbrauch des kontinuierlichen Systems ab. Was sagt dir diese Differenz über die Effizienz deines Entwurfs? Wie könnten sich die Wassereinsparungen deines Entwurfs auf die landwirtschaftlichen Praktiken in Gebieten mit Wasserknappheit auswirken?

## Herzlichen Glückwunsch! @showdialog

Du hast hast diese Aktivität abgeschlossen!

## Analyse @showdialog

Bevor wir zum Schluss kommen:

Nenne eine Sache, die du heute gelernt hast?

## Fertig!

Du kannst auf die Schaltfläche `|Done|` klicken, um das Tutorial zu beenden.

Besuch auch mal calliope.cc, um weitere inspirierende Ideen und Projekte zu entdecken!
