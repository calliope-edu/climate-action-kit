# Windkraftanlage - Tutorial

```package
fwd-climate-action=github:calliope-edu/climate-action-kit
datalogger=datalogger
```

```template
fwdButtons.dialButton1.onEvent(jacdac.ButtonEvent.Down, function () {
    fwdMotors.conSetEnabled(fwdBase.middleServo, false)
})
input.onButtonEvent(Button.A, input.buttonEventClick(), function () {
    basic.showNumber(Batteriestand)
})
fwdButtons.dial1.onRotated(fwdEnums.ClockwiseCounterclockwise.Clockwise, function () {
    fwdMotors.setSpeed(fwdBase.middleServo, -50)
})
fwdButtons.dial1.onRotated(fwdEnums.ClockwiseCounterclockwise.Counterclockwise, function () {
    fwdMotors.setSpeed(fwdBase.middleServo, 50)
})
let Batteriestand = 0
Batteriestand = 0
basic.forever(function () {
    if (fwdMotors.conIsEnabled(fwdBase.middleServo) == true) {
        basic.showLeds(`
            . . # . .
            . # # # .
            # # # # #
            . # . # .
            . # # # .
            `)
        Batteriestand += 1
        if (Batteriestand > 100) {
            Batteriestand = 100
        }
        basic.pause(2000)
    } else {
        basic.showLeds(`
            . . . . .
            . . . . .
            . . . . .
            . . . . .
            . . . . .
            `)
    }
})
```

## Aktivität 1: Erstelle dein Projekt @showdialog

Lasst uns eine automatisierte Windkraftanlage bauen. Wir werden dies in vier Schritten tun:

1. **Bauen:** Den Prototypen konstruieren
2. **Code erstellen:** Das Projekt zum Leben erwecken
3. **Ausprobieren:** Herausfinden, ob der fertige Prototyp funktioniert
4. **Modifizieren:** Das Projekt mit einer kleinen Programmieraufgabe verändern

<img src="https://raw.githubusercontent.com/calliope-edu/climate-action-kit/main/tutorial-assets/ms-windsample-render.webp" alt="Full sample wind tubine render" style="display: block; width: 60%; margin:auto;">

## Bauanleitung Schritt 1 @showdialog

![sbs1](https://raw.githubusercontent.com/calliope-edu/climate-action-kit/main/tutorial-assets/ms-windsample-sbs01.webp)

## Bauanleitung Schritt 2 @showdialog

![sbs1](https://raw.githubusercontent.com/calliope-edu/climate-action-kit/main/tutorial-assets/ms-windsample-sbs02.webp)

## Bauanleitung Schritt 3 @showdialog

![sbs1](https://raw.githubusercontent.com/calliope-edu/climate-action-kit/main/tutorial-assets/ms-windsample-sbs03.webp)

## Bauanleitung Schritt 4 @showdialog

![sbs1](https://raw.githubusercontent.com/calliope-edu/climate-action-kit/main/tutorial-assets/ms-windsample-sbs04.webp)

## Bauanleitung Schritt 5 @showdialog

![sbs1](https://raw.githubusercontent.com/calliope-edu/climate-action-kit/main/tutorial-assets/ms-windsample-sbs05.webp)

## Bauanleitung Schritt 6 @showdialog

![sbs1](https://raw.githubusercontent.com/calliope-edu/climate-action-kit/main/tutorial-assets/ms-windsample-sbs06.webp)

## Bauanleitung Schritt 7 @showdialog

![sbs1](https://raw.githubusercontent.com/calliope-edu/climate-action-kit/main/tutorial-assets/ms-windsample-sbs07.webp)

## Bauanleitung Schritt 8 @showdialog

![sbs1](https://raw.githubusercontent.com/calliope-edu/climate-action-kit/main/tutorial-assets/ms-windsample-sbs08.webp)

## Bauanleitung Schritt 9 @showdialog

![sbs1](https://raw.githubusercontent.com/calliope-edu/climate-action-kit/main/tutorial-assets/ms-windsample-sbs09.webp)

## Bauanleitung Schritt 10 @showdialog

![sbs1](https://raw.githubusercontent.com/calliope-edu/climate-action-kit/main/tutorial-assets/ms-windsample-sbs10.webp)

## Aktivität 2: Code erstellen @showdialog

Wir müssen unser Modell mit dem Computer verbinden, damit es mit Code zum Leben erweckt werden kann!

Der Code enthält die Anweisungen, die unserem Calliope mini sagen, was er tun soll.

## Code Schritt 1 @showdialog

WICHTIG! Vergewissere sich, dass dein Climate Action Kit Breakout Board eingeschaltet und der Calliope mini an einem Computer angeschlossen ist.
<img src="https://raw.githubusercontent.com/calliope-edu/climate-action-kit/main/tutorial-assets/pluganim.webp" alt="Plug Calliope mini into USB port on computer" style="display: block; width: 40%; margin:auto;">

## Code Schritt 2 @showdialog

Klicke auf die drei Punkte neben der Schaltfläche `|Download|` und dann auf „Gerät verbinden“.
Befolge anschließend die Schritte zum Koppeln des Calliope mini.

<img src="https://raw.githubusercontent.com/calliope-edu/climate-action-kit/main/tutorial-assets/pairmicrobitGIF.webp"  alt="Pairing gif" style="display: block; width: 60%; margin:auto;">

## Code Schritt 3

Klicke anschließend auf die Schaltfläche `|Download|`, um den Code vom Projekt herunterzuladen.

## Aktivität 3: Ausprobieren @showdialog

Das Tutorial ermöglicht es, Lernen in drei Projektphasen zu strukturieren: **Verwenden, Modifizieren und Erstellen.**

Nachdem wir nun unsere Windkraftanlage gebaut haben, beginnen wir damit, den Beispielcode zu **verwenden**, um zu sehen, wie sie funktioniert.

Während du die nächsten Schritte durchgehst:

- **Verwende** die Anweisungen oben auf dem Bildschirm.
- Wenn du weitere Informationen benötigst, klicke auf **„Mehr erfahren!“**.
- Wenn du Hilfe beim Code benötigst, klicke auf die **Glühbirne**!

<img src="https://raw.githubusercontent.com/calliope-edu/climate-action-kit/main/tutorial-assets/tellmore_hintbox_gif.webp" style="display: block; width: 80%; margin:auto;">


## Ausprobieren Schritt 1

Sieh dir die Wind­kraft­anlage genau an. Kannst du alle ihre Teile benennen? Was macht jeder Teil

~hint Mehr erfahren!
Dieses Modell benutzt:

-   **Bauteile:** eine Bodenplatte, einen Würfel-Verbinder, einen langen weißen Rahmen, einen grünen Kreis, vier kleine grüne Rahmen, vier Rücken-an-Rücken-Verbinder. Diese Bauteile helfen dir, die Struktur der Windkraftanlage zu bauen.
-   **Roboter-Teile:** ein Breakout-Board, einen Calliope mini, einen kontinuierlichen Servo-Motor und einen Drehknopf. Diese Teile lassen deine Windkraftanlage bewegen!
    hint~

## Ausprobieren Schritt 2

Bevor wir den Code testen, machen wir ein paar _Vorhersagen_:

-   Was glaubst du, passiert, wenn du den Drehknopf im Uhrzeigersinn drehst? Und was passiert gegen den Uhrzeigersinn?
-   Was passiert, wenn du den Drehknopf nach unten drückst?

Schau dir den Code genau an!

## Ausprobieren Schritt 3

Probieren wir es aus!

Drehe den Drehknopf im Uhrzeigersinn oder gegen den Uhrzeigersinn. Drücke ihn danach nach unten. Was passiert?

~hint Mehr erfahren!

-   Wenn du den Drehknopf drehst, dreht sich die Turbine in die gleiche Richtung. Auf den LEDs siehst du auch ein Haus.
-   Wenn du den Drehknopf nach unten drückst, hört die Turbine auf sich zu drehen und das Haus verschwindet.
-   Das zeigt dir, wie Windkraftanlagen Strom erzeugen und Häuser mit Strom versorgen, wenn sie sich drehen!
    hint~

## Ausprobieren Schritt 4

Wir benutzen zwei `||fwdButtons:on dial rotated||` **Ereignisse**, damit sich die Windkraftanlage dreht. Das `||fwdButtons:on dial down||` **Ereignis** stoppt die Turbine.

In diesem Beispiel steht der Drehknopf für den Wind!

```blocks
fwdButtons.dial1.onRotated(fwdEnums.ClockwiseCounterclockwise.Counterclockwise, function () {
    fwdMotors.setSpeed(fwdBase.middleServo, 50)
})
fwdButtons.dial1.onRotated(fwdEnums.ClockwiseCounterclockwise.Clockwise, function () {
    fwdMotors.setSpeed(fwdBase.middleServo, -50)
})

fwdButtons.dialButton1.onEvent(jacdac.ButtonEvent.Down, function () {
    fwdMotors.conSetEnabled(fwdBase.middleServo, false)
})
```

## Ausprobieren Schritt 5

Wir benutzen eine **Wenn-dann-Bedingung**, um die Haustiere einzuschalten, wenn die Turbine Strom erzeugt.

Erkennst du die Wenn-dann-Bedingung im Code?

~hint Mehr erfahren!

-   Wenn-dann-Anweisungen sind Regeln, die dem Calliope mini helfen, Entscheidungen zu treffen. Solche Regeln benutzen wir auch im echten Leben! Zum Beispiel: „Wenn es regnet, dann mache ich meinen Regenschirm auf!“
-   Hier haben wir dem Calliope mini gesagt: „Wenn sich die Windkraftanlage dreht, dann soll das Haus leuchten!“
    hint~

```block
if (fwdMotors.conIsEnabled(fwdBase.middleServo) == true) {
        basic.showLeds(`
            . . # . .
            . # # # .
            # # # # #
            . # . # .
            . # # # .
            `)
    } else {
        basic.showLeds(`
            . . . . .
            . . . . .
            . . . . .
            . . . . .
            . . . . .
            `)
    }
```

## Ausprobieren Schritt 6

Sieh dir deinen Code noch einmal an. Was glaubst du, passiert, wenn du A drückst?

Probier es jetzt aus.

~hint Mehr erfahren!

-   Wenn du A drückst, zeigt der Calliope mini für einen Moment eine Zahl auf der LED-Matrix an.
    hint~

```blocks
input.onButtonPressed(Button.A, function () {
    basic.showNumber(Batteriestand)
})
```

## Ausprobieren Schritt 7

Lass deine Windkraftanlage 10 Sekunden lang laufen. Drücke dann noch einmal A. Was ist mit der Zahl auf der LED-Matrix passiert?

~hint Mehr erfahren!

-   Die Zahl ist größer geworden!
    hint~

## Ausprobieren Schritt 8

Immer wenn sich unsere Windkraftanlage dreht, versorgt sie das Haus mit Strom und „lädt“ gleichzeitig langsam eine Batterie auf.

Wir haben in unserem Programm eine **Variable** erstellt, um den Batteriestand zu verfolgen. Am Anfang des Programms ist der `||variables:Batteriestand||` '0'. AWährend sich die Turbine dreht, steigt der Stand alle 2 Sekunden um 1%.

~hint Mehr erfahren!

-   Der Block `||variables:ändere Batteriestand um 1||` erhöht die Variable um 1. Das passiert alle 2 Sekunden wegen des `||basic:pausieren||` Blocks.
-   So wird simuliert, wie echte Windkraftanlagen Energie in Batterien speichern, um sie später zu nutzen.
    hint~

```blocks
// @highlight
Batteriestand = 0
basic.forever(function () {
    if (fwdMotors.conIsEnabled(fwdBase.middleServo) == true) {
        basic.showLeds(`
            . . # . .
            . # # # .
            # # # # #
            . # . # .
            . # # # .
            `)
        // @highlight
        Batteriestand += 1
        // @highlight
        basic.pause(2000)
    } else {
        basic.showLeds(`
            . . . . .
            . . . . .
            . . . . .
            . . . . .
            . . . . .
            `)
    }
})
```

## Ausprobieren Schritt 9

Die Batterie startet bei 0% und lädt alle 2 Sekunden um 1% auf. Wir wollen wissen, wie lange es dauert, bis sie 100% erreicht.

Wie könnte man das Problem lösen?

## Ausprobieren Schritt 10

Lade den Code noch einmal herunter, um deine Batterie zurückzusetzen.
Drehe dann den Drehknopf und beobachte, wie lange es dauert, bis die Batterie 100% erreicht. War deine Rechnung richtig?

## Herzlichen Glückwunsch! @showdialog

Du hast hast diese Aktivität abgeschlossen!

## Analyse @showdialog

Nenne eine Sache, die du heute gelernt hast?

## Fertig!

Du kannst auf die Schaltfläche `|Done|` klicken, um das Tutorial zu beenden.

Auf der Internetseite **calliope.cc** findest du weitere inspirierende Ideen und Projekte!