# Optimierung des Pflanzenwachstums mit LED-Wachstumslampen

```package
fwd-climate-action=github:calliope-edu/climate-action-kit#v1.1.0
```

## Aktivität 1: Erstelle dein Projekt @showdialog
Lasst uns einen Prototyp einer vertikalen Farm bauen! Wir werden dies in drei Teilen tun:

1. **Bauen:** Den Prototypen konstruieren
2. **Code erstellen:** Das Projekt zum Leben zu erwecken
3. **Ausprobieren:** Herausfinden, ob der Prototyp unserer vertikalen Farm funktioniert

<img src="https://raw.githubusercontent.com/calliope-edu/climate-action-kit/main/tutorial-assets/gr9-verticalfarm-thumbnail-render.webp" alt="Full vertical farm render" style="display: block; width: 60%; margin:auto;">

## Bauanleitung Schritt 1 @showdialog

![verticalfarmsbs](https://raw.githubusercontent.com/calliope-edu/climate-action-kit/main/tutorial-assets/gr9-verticalfarm-sbs01.webp)

## Bauanleitung Schritt 2 @showdialog

![verticalfarmsbs](https://raw.githubusercontent.com/calliope-edu/climate-action-kit/main/tutorial-assets/gr9-verticalfarm-sbs02.webp)

## Bauanleitung Schritt 3 @showdialog

![verticalfarmsbs](https://raw.githubusercontent.com/calliope-edu/climate-action-kit/main/tutorial-assets/gr9-verticalfarm-sbs03.webp)

## Bauanleitung Schritt 4 @showdialog

![verticalfarmsbs](https://raw.githubusercontent.com/calliope-edu/climate-action-kit/main/tutorial-assets/gr9-verticalfarm-sbs04.webp)

## Bauanleitung Schritt 5 @showdialog

![verticalfarmsbs](https://raw.githubusercontent.com/calliope-edu/climate-action-kit/main/tutorial-assets/gr9-verticalfarm-sbs05.webp)

## Bauanleitung Schritt 6 @showdialog

![verticalfarmsbs](https://raw.githubusercontent.com/calliope-edu/climate-action-kit/main/tutorial-assets/gr9-verticalfarm-sbs06.webp)

## Bauanleitung Schritt 7 @showdialog

![verticalfarmsbs](https://raw.githubusercontent.com/calliope-edu/climate-action-kit/main/tutorial-assets/gr9-verticalfarm-sbs07.webp)

## Bauanleitung Schritt 8 @showdialog

![verticalfarmsbs](https://raw.githubusercontent.com/calliope-edu/climate-action-kit/main/tutorial-assets/gr9-verticalfarm-sbs08.webp)

## Bauanleitung Schritt 9 @showdialog

![verticalfarmsbs](https://raw.githubusercontent.com/calliope-edu/climate-action-kit/main/tutorial-assets/gr9-verticalfarm-sbs09.webp)

## Bauanleitung Schritt 10 @showdialog

![verticalfarmsbs](https://raw.githubusercontent.com/calliope-edu/climate-action-kit/main/tutorial-assets/gr9-verticalfarm-sbs10.webp)

## Bauanleitung Schritt 11 @showdialog

![verticalfarmsbs](https://raw.githubusercontent.com/calliope-edu/climate-action-kit/main/tutorial-assets/gr9-verticalfarm-sbs11.webp)

## Bauanleitung Schritt 12 @showdialog

![verticalfarmsbs](https://raw.githubusercontent.com/calliope-edu/climate-action-kit/main/tutorial-assets/gr9-verticalfarm-sbs12.webp)

## Bauanleitung Schritts 13 + 14 @showdialog

![verticalfarmsbs](https://raw.githubusercontent.com/calliope-edu/climate-action-kit/main/tutorial-assets/gr9-verticalfarm-sbs13.webp)

## Bauanleitung Schritt 15 @showdialog

![verticalfarmsbs](https://raw.githubusercontent.com/calliope-edu/climate-action-kit/main/tutorial-assets/gr9-verticalfarm-sbs15.webp)

## Bauanleitung Schritt 16 @showdialog

![verticalfarmsbs](https://raw.githubusercontent.com/calliope-edu/climate-action-kit/main/tutorial-assets/gr9-verticalfarm-sbs16.webp)

## Bauanleitung Schritt 17 @showdialog

![verticalfarmsbs](https://raw.githubusercontent.com/calliope-edu/climate-action-kit/main/tutorial-assets/gr9-verticalfarm-sbs17.webp)

## Bauanleitung Schritt 18 @showdialog

![verticalfarmsbs](https://raw.githubusercontent.com/calliope-edu/climate-action-kit/main/tutorial-assets/gr9-verticalfarm-sbs18.webp)

## Bauanleitung Schritt 19 @showdialog

![verticalfarmsbs](https://raw.githubusercontent.com/calliope-edu/climate-action-kit/main/tutorial-assets/gr9-verticalfarm-sbs19.webp)

## Bauanleitung Schritt 20 @showdialog

![verticalfarmsbs](https://raw.githubusercontent.com/calliope-edu/climate-action-kit/main/tutorial-assets/gr9-verticalfarm-sbs20.webp)

## Bauanleitung Schritt 21 @showdialog

![verticalfarmsbs](https://raw.githubusercontent.com/calliope-edu/climate-action-kit/main/tutorial-assets/gr9-verticalfarm-sbs21.webp)

## Aktivität 2: Code Your Project @showdialog

Wir müssen unser Modell mit dem Computer verbinden, damit es mit Code zum Leben erweckt werden kann!

Der Code enthält die Anweisungen, die unserem Calliope mini sagen, was er tun soll.

```template
input.onButtonPressed(Button.A, function () {
    fwdBase.leftServo.setAngleAndWait(10)
    basic.showLeds(`
        # . # . #
        . # # # .
        # # # # #
        . # # # .
        # . # . #
        `)
    fwdLights.ledRing1.setAllPixelsColor(0xff0000)
    basic.pause(5000)
    fwdLights.ledRing1.setAllPixelsColor(0x000000)
    basic.clearScreen()
    fwdBase.leftServo.setAngleAndWait(0)
    basic.pause(5000)
})
input.onButtonPressed(Button.B, function () {
    fwdBase.leftServo.setAngleAndWait(60)
    basic.showLeds(`
        # . # . #
        . # # # .
        # # # # #
        . # # # .
        # . # . #
        `)
    fwdLights.ledRing1.setAllPixelsColor(0x0000ff)
    basic.pause(5000)
    fwdLights.ledRing1.setAllPixelsColor(0x000000)
    basic.clearScreen()
    fwdBase.leftServo.setAngleAndWait(0)
    basic.pause(5000)
})
input.onButtonPressed(Button.AB, function () {
    fwdBase.leftServo.setAngleAndWait(120)
    basic.showLeds(`
        # . # . #
        . # # # .
        # # # # #
        . # # # .
        # . # . #
        `)
    fwdLights.ledRing1.setAllPixelsColor(0xffffff)
    basic.pause(5000)
    fwdLights.ledRing1.setAllPixelsColor(0x000000)
    basic.clearScreen()
    fwdBase.leftServo.setAngleAndWait(0)
    basic.pause(5000)
})

fwdBase.leftServo.setAngleAndWait(0)

// @collapsed
function lightPlant (location: number, colour: number) {
    fwdBase.leftServo.setAngleAndWait(location)
    basic.showLeds(`
        # . # . #
        . # # # .
        # # # # #
        . # # # .
        # . # . #
        `)
    fwdLights.ledRing1.setAllPixelsColor(colour)
    basic.pause(5000)
    fwdLights.ledRing1.setAllPixelsColor(0x000000)
    basic.clearScreen()
    fwdBase.leftServo.setAngleAndWait(0)
    basic.pause(5000)
}

// @collapsed
input.onLogoEvent(TouchButtonEvent.Pressed, function () {
    lightPlant(10, 16711680)
})
```

## Code Step 1 @showdialog

WICHTIG! Vergewissere dich, dass dein Climate Action Kit Breakout Board eingeschaltet und dein Calliope mini an einem Computer angeschlossen ist.

<img src="https://raw.githubusercontent.com/calliope-edu/climate-action-kit/main/tutorial-assets/pluganim.webp" alt="Turn on breakout board" style="display: block; width: 40%; margin:auto;">

## Code Step 2 @showdialog

Klicke auf die drei Punkte neben der Schaltfläche `|Download|` und dann auf „Gerät verbinden“.
Befolge anschließend die Schritte zum Koppeln des Calliope mini.

<img src="https://raw.githubusercontent.com/calliope-edu/climate-action-kit/main/tutorial-assets/pairmicrobitGIF.webp" alt="Full wildfire render" style="display: block; width: 60%; margin:auto;">

## Code Step 3

Klicke anschließend auf die Schaltfläche `|Download|`, um den Code vom Projekt herunterzuladen.

## Aktivität 3: Use Your Project @showdialog

Wir sind bereit, unseren **Prototyp** einer vertikalen Farm einzusetzen!

~hint 
- **Verwende** die Anweisungen oben auf dem Bildschirm.
- Wenn du weitere Informationen benötigst, klicke auf **„Mehr erfahren!“** ().
- Wenn du Hilfe beim Code benötigst, klicke auf die **Glühbirne**!

## Ausprobieren Schritt 1

Schaue dir deinen Prototyp der vertikalen Farm an. Kannst du alle seiner physischen Teile benennen?

~hint Mehr erfahren!
Unsere vertikale Farm verfügt über:

-   **Bausteine**: eine Grundplatte, zwei lange Rahmen, einen mittleren Rahmen, vier kleine Rahmen, einen Kreis, drei Würfelverbinder und drei Eckverbinder
-   **Robotikkomponenten**: einen Calliope mini, eine Breakout-Platine, eine Batterie, einen Positionsservomotor und einen LED-Ring
-   Einen langen Kabelverbinder
    hint~

## Ausprobieren Schritt 2

Was ist deiner Meinung nach der Zweck der einzelnen Teile? Wie wirken sie miteinander?

~hint Mehr erfahren!
- Die **Bausteine** bilden die Stapel, die die Pflanzen in unserer vertikalen Farm halten, sowie den LED-Arm, der unsere Pflanzen beleuchtet.
- Der **Calliope mini** speichert den gesamten Code, der unserem vertikalen Farming-Prototyp mitteilt, wie er zu funktionieren hat.
- Das **Breakout-Board** sendet diese Anweisungen vom Calliope mini an den **LED-Ring** und den **Positionsservomotor**. Der Positionsservomotor dreht unseren LED-Arm, sodass er sich zu einer bestimmten Pflanzenreihe bewegen und diese beleuchten kann.
- Die **Batterie** auf dem Breakout-Board versorgt unser Projekt mit Strom, wenn es nicht an den Computer angeschlossen ist.
    hint~

## Ausprobieren Schritt 3

Beginnen wir damit, unsere vertikale Farm zu testen.

Was passiert, wenn du A drückst? Drücke die Taste mehrmals und schreiben eine geordnete Liste mit allem auf, was dir auffällt.

_Hinweis: Warte zwischen jedem Tastendruck 5 Sekunden._

~hint Mehr erfahren!
Wenn du A drückst:

1. Der LED-Arm bewegt sich neben die oberste Pflanzenreihe.
2. Der Calliope mini zeigt ein Sonnensymbol auf seinem LED-Display an.
3. Der LED-Ring leuchtet etwa 5 Sekunden lang rot.
4. Der LED-Ring erlischt.
5. Die LED-Anzeige des Calliope mini wird gelöscht.
6. Der LED-Arm bewegt sich zurück in seine Ausgangsposition.

Dies ist die ideale Beleuchtung für die Pflanze, die sich auf der obersten Etage unserer vertikalen Farm befindet.
hint~

## Ausprobieren Schritt 4

Was passiert, wenn du B drückst? Drücke die Taste mehrmals und schreibe eine geordnete Liste mit allem auf, was dir auffällt.

_Hinweis: Warte zwischen jedem Tastendruck 5 Sekunden._

~hint Mehr erfahren!
Wenn du B drückst:

1. Der LED-Arm bewegt sich neben die mittlere Pflanzenreihe.
2. Der Calliope mini zeigt ein Sonnensymbol auf seinem LED-Display an.
3. Der LED-Ring leuchtet etwa 5 Sekunden lang blau.
4. Der LED-Ring erlischt.
5. Die LED-Anzeige des Calliope mini wird gelöscht.
6. Der LED-Arm bewegt sich zurück in seine Ausgangsposition.

Dies ist die ideale Beleuchtung für die Pflanze, die sich auf dem mittleren Stapel in unserer vertikalen Farm befindet.
hint~

## Ausprobieren Schritt 5

Was passiert, wenn du A+B drückst? Drücke die Tasten mehrmals gleichzeitig und schreibe eine geordnete Liste mit allem auf, was dir auffällt.

_Hinweis: Warte zwischen jedem Tastendruck 5 Sekunden._

~hint Mehr erfahren!
Wenn du A+B drückst:

1. Der LED-Arm bewegt sich neben die untere Pflanzenreihe.
2. Der Calliope mini zeigt ein Sonnensymbol auf seinem LED-Display an.
3. Der LED-Ring leuchtet etwa 5 Sekunden lang weiß.
4. Der LED-Ring erlischt.
5. Die LED-Anzeige des Calliope mini wird gelöscht.
6. Der LED-Arm bewegt sich zurück in seine Ausgangsposition.

Dies ist die ideale Beleuchtung für die Pflanze, die sich auf der untersten Etage unserer vertikalen Farm befindet.
hint~

## Ausprobieren Schritt 6

Vergleiche und kontrastiere diese Beleuchtungsarten. Was ist unterschiedlich? Was ist gleich?
An dieser Stelle kannst du dir den Code unter den `||input:on button A pressed||`, `||input:on button B pressed||`, und `||input:on button A+B pressed||` Blöcken auf der Bühne anschauen, wenn es hilft!

~hint Mehr erfahren!
Die Beleuchtung für jede Pflanze ist nahezu identisch. Die einzigen Unterschiede sind:

1. die Position des LED-Arms, um die jeweiligen Pflanzen optimal zu erreichen (der Winkel des Positionsservomotors)
2. die Farbe der LEDs
   hint~

## Ausprobieren Schritt 7

Es ist nicht sehr effizient, dieselben Anweisungen mehrmals zu schreiben! Außerdem könnte ohne einen Namen der Zweck all dieser Schritte für jemanden, der nur einen kurzen Blick auf den Code wirft, unklar sein.

Wie könntest du eine einzige Abfolge von Schritten schreiben, die zur Behandlung aller Pflanzen verwendet werden könnte? Wie würdest du diesen Prozess nennen? Probiere es jetzt aus!

~Hinweis Mehr erfahren!
Nennen wir diesen Prozess: Pflanzenlichtbehandlung.

Wir könnten Platzhalter für Werte verwenden, die sich je nach Pflanzenart oder Lebensphase ändern können! Zum Beispiel, um eine Pflanze zu beleuchten:

1. Der LED-Arm bewegt sich neben die (**Position**) der Pflanzen.
2. Der Calliope mini zeigt ein Sonnensymbol auf seinem LED-Display an.
3. Der LED-Ring leuchtet etwa 5 Sekunden lang in (**Farbe**).
4. Der LED-Ring schaltet sich aus.
5. Die LED-Anzeige des Calliope mini wird gelöscht.
6. Der LED-Arm bewegt sich zurück in seine Ausgangsposition.
   hint~

## Ausprobieren Schritt 8

Wir können dies beim Programmieren erreichen, indem wir eine **Funktion** schreiben! Eine Funktion ist ein Block wiederverwendbaren Codes, der eine einzelne Aktion ausführt. In diesem Fall ist diese Aktion das Beleuchten unserer verschiedenen Pflanzen!

Wir haben eine Funktion für dich vorab geschrieben. Klicke auf den Pfeil neben dem blauen Block, um den Code zu erweitern!

~hint Mehr erfahren!

-   Beachte, dass die Reihenfolge der Schritte dieselbe ist wie unter jedem Ereignis, außer dass wir jetzt Variablen für alle Werte verwenden, die sich ändern!
    hint~

```blocks
function lightPlant (location: number, colour: number) {
    fwdBase.leftServo.setAngleAndWait(location)
    basic.showLeds(`
        # . # . #
        . # # # .
        # # # # #
        . # # # .
        # . # . #
        `)
    fwdLights.ledRing1.setAllPixelsColor(colour)
    basic.pause(5000)
    fwdLights.ledRing1.setAllPixelsColor(0x000000)
    basic.clearScreen()
    fwdBase.leftServo.setAngleAndWait(0)
    basic.pause(5000)
}
```

## Ausprobieren Schritt 9

Wenn du eine Funktion in deinem Code verwenden möchten, musst du sie aufrufen.
~hint Mehr erfahren!

-   Du findest die `||functions:call lightPlant||` Block unter dem `||functions:Functions||` Kategorie.
    hint~

## Ausprobieren Schritt 10

Wir haben bereits ein`||functions:call lightPlant||` Block zu unserem Code unter dem `||input:on logo touched||` Ereignis. Erweitere diesen Code, indem du auf den Abwärtspfeil klickst.

Drücke erneut auf A und berühre dann das Logo auf der Vorderseite des Calliope mini. Was fällt dir auf?

_Hinweis: Warte zwischen dem Drücken der Taste und dem Berühren des Logos 5 Sekunden._
~hint Mehr erfahren!

-   Hoffentlich ist dir aufgefallen, dass die Beleuchtung genauso ist wie zuvor!
    hint~

```blocks
// @hide
function lightPlant (location: number, colour: number) {
    fwdBase.leftServo.setAngleAndWait(location)
    basic.showLeds(`
        # . # . #
        . # # # .
        # # # # #
        . # # # .
        # . # . #
        `)
    fwdLights.ledRing1.setAllPixelsColor(colour)
    basic.pause(5000)
    fwdLights.ledRing1.setAllPixelsColor(0x000000)
    basic.clearScreen()
    fwdBase.leftServo.setAngleAndWait(0)
    basic.pause(5000)
}


input.onLogoEvent(TouchButtonEvent.Pressed, function () {
    lightPlant(10, 16711680)
})
```

## Ausprobieren Schritt 11

Siehst du, wie viel einfacher der Code jetzt zu interpretieren ist?

Durch die Verwendung einer Funktion können wir unseren Code vereinfachen, ihn lesbarer machen und die Anzahl der verwendeten Blöcke reduzieren! Jedes Ereignis benötigt nur noch 1 Block statt 8!
## Herzlichen Glückwunsch! @showdialog

Du hast hast diese Aktivität abgeschlossen!

## Analyse @showdialog

Bevor wir zum Schluss kommen:

Nenne zwei neue Dinge, die du heute gelernt hast.

Was ist eine Sache, über die du mehr erfahren möchtest?

## Fertig!

Du kannst auf die Schaltfläche `|Done|` klicken, um das Tutorial zu beenden.

Besuch auch mal calliope.cc, um weitere inspirierende Ideen und Projekte zu entdecken!