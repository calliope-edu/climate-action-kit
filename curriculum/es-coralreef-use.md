# Coral Reef Model - Use Tutorial

```package
fwd-climate-action-kit=github:calliope-edu/climate-action-kit
datalogger=datalogger
```

```template
fwdButtons.dial1.onRotated(fwdEnums.ClockwiseCounterclockwise.Counterclockwise, function () {
    temperature += -1
})
fwdButtons.dial1.onRotated(fwdEnums.ClockwiseCounterclockwise.Clockwise, function () {
    temperature += 1
})
let temperature = 28
basic.forever(function () {
    basic.showNumber(temperature)
})
basic.forever(function () {
    if (temperature > 30) {
        fwdLights.ledRing1.setAllPixelsColor(0xffffff)
    } else {
        fwdLights.ledRing1.setAllPixelsColor(0xff0080)
    }
    basic.pause(100)
})
```

## Aktivität 1: Erstelle dein Projekt @showdialog

Lasst uns unser Korallenriff-Modell bauen! Wir werden dies in drei Schritten tun:

1. **Bauen:** Den Prototypen konstruieren
2. **Code erstellen:** Das Projekt zum Leben zu erwecken
3. **Ausprobieren:** Herausfinden, ob der fertige Prototyp funktioniert

<img src="https://raw.githubusercontent.com/calliope-edu/climate-action-kit/main/tutorial-assets/es-coralreef-render.webp" alt="Full coral reef model render" style="display: block; width: 70%; margin:auto;">

## Bauanleitung Schritt 1 @showdialog

![sbs1](https://raw.githubusercontent.com/calliope-edu/climate-action-kit/main/tutorial-assets/es-coralreef-sbs01.webp)

## Bauanleitung Schritt 2 @showdialog

![sbs2](https://raw.githubusercontent.com/calliope-edu/climate-action-kit/main/tutorial-assets/es-coralreef-sbs02.webp)

## Bauanleitung Schritt 3 @showdialog

![sbs3](https://raw.githubusercontent.com/calliope-edu/climate-action-kit/main/tutorial-assets/es-coralreef-sbs03.webp)

## Bauanleitung Schritt 4 @showdialog

![sbs4](https://raw.githubusercontent.com/calliope-edu/climate-action-kit/main/tutorial-assets/es-coralreef-sbs04.webp)

## Bauanleitung Schritt 5 @showdialog

![sbs5](https://raw.githubusercontent.com/calliope-edu/climate-action-kit/main/tutorial-assets/es-coralreef-sbs05.webp)

## Bauanleitung Schritt 6 @showdialog

![sbs6](https://raw.githubusercontent.com/calliope-edu/climate-action-kit/main/tutorial-assets/es-coralreef-sbs06.webp)

## Bauanleitung Schritt 7 @showdialog

![sbs7](https://raw.githubusercontent.com/calliope-edu/climate-action-kit/main/tutorial-assets/es-coralreef-sbs07.webp)

## Bauanleitung Schritt 8 @showdialog

![sbs8](https://raw.githubusercontent.com/calliope-edu/climate-action-kit/main/tutorial-assets/es-coralreef-sbs08.webp)

## Bauanleitung Schritt 9 @showdialog

![sbs9](https://raw.githubusercontent.com/calliope-edu/climate-action-kit/main/tutorial-assets/es-coralreef-sbs09.webp)

## Bauanleitung Schritt 10 @showdialog

![sbs10](https://raw.githubusercontent.com/calliope-edu/climate-action-kit/main/tutorial-assets/es-coralreef-sbs10.webp)

## Bauanleitung Schritt 11 @showdialog

![sbs11](https://raw.githubusercontent.com/calliope-edu/climate-action-kit/main/tutorial-assets/es-coralreef-sbs11.webp)

## Bauanleitung Schritt 12 @showdialog

![sbs12](https://raw.githubusercontent.com/calliope-edu/climate-action-kit/main/tutorial-assets/es-coralreef-sbs12.webp)

## Aktivität 2: Code erstellen @showdialog

Wir müssen unser Modell mit dem Computer verbinden, damit es mit Code zum Leben erweckt wird!

Der Code enthält die Anweisungen, die unserem Calliope mini sagen, was er tun soll.

## Code Schritt 1 @showdialog

WICHTIG! Vergewissere dich, dass dein Climate Action Kit Breakout Board eingeschaltet und dein Calliope mini an einem Computer angeschlossen ist.

<img src="https://raw.githubusercontent.com/calliope-edu/climate-action-kit/main/tutorial-assets/pluganim.webp" alt="Plug Calliope mini into USB port on computer" style="display: block; width: 40%; margin:auto;">

## Code Schritt 2 @showdialog

Klicke auf die drei Punkte neben der Schaltfläche `|Download|` und dann auf „Gerät verbinden“.
Befolge anschließend die Schritte zum Koppeln des Calliope mini.

<img src="https://raw.githubusercontent.com/calliope-edu/climate-action-kit/main/tutorial-assets/pairmicrobitGIF.webp"  alt="Pairing gif" style="display: block; width: 60%; margin:auto;">

## Code schritt 3

Klicke anschließend auf die Schaltfläche `|Download|`, um den Code vom Projekt herunterzuladen.

## Aktivität 3: Ausprobieren @showdialog

Wir sind nun bereit, unser Korallenriffmodell **auszuprobieren**, um zu sehen, wie es zu Korallenbleiche kommt, wenn das Wasser zu warm wird.

**Tipps**

1. **Folge** den Schritten oben auf dem Bildschirm.
2. Wenn du weitere Informationen benötigst, klicke auf **„Mehr erfahren!“**.
3. Wenn du Hilfe mit dem Code benötigst, klicke auf die **Glühbirne!**
<img src="https://raw.githubusercontent.com/calliope-edu/climate-action-kit/main/tutorial-assets/tellmore_hintbox_gif.webp" style="display: block; width: 80%; margin:auto;">

## Ausprobieren Schritt 1

Schau dir das Modell, das du gerade gebaut hast, genau an. Kannst du die verschiedenen Teile benennen, die du dafür verwendet hast? Sei dabei möglichst genau!
~hint Mehr erfahren!
Dieses Modell verwendet:

-   **Bausteine:** Eine Grundplatte, einen Kreis, vier Würfelverbinder und zwei mittelgroße weiße Rahmen
-   **Bastelmaterial:** Seidenpapier
-   **Roboterteile:** Eine Breakout-Platine, Calliope mini, Drehregler und LED-Ring
    hint~

## Ausprobieren Schritt 2

Was glaubst du, was die verschiedenen Teile des Modells darstellen?
~hint Mehr erfahren!

-   Der LED-Ring stellt die Koralle dar. Seine Farbe zeigt an, ob die Koralle gesund oder gebleicht ist. Wir verwenden Seidenpapier, damit der LED-Ring noch mehr wie eine Koralle aussieht. Es stellt die Tentakel des Korallenpolypen dar!
    hint~

## Ausprobieren Schritt 4

Es ist an der Zeit, das Modell zu testen, indem du den Drehknopf langsam um eine Stufe nach rechts drehst.
Was fällt dir auf?
~hint Mehr erfahren!

- Die Zahl auf dem LED-Bildschirm des Calliope mini hat sich um 1 erhöht.
- Diese Zahl gibt die aktuelle Temperatur des Ozeans an.
    hint~

## Ausprobieren Schritt 5

Wir verwenden eine **Variable**, um die Temperatur zu speichern. Variablen sind wie Kisten, die Informationen für uns aufbewahren.

Jedes Mal, wenn du den Drehknopf drehst, ändert sich die Temperaturvariable entsprechend der Drehrichtung. Versuche, den Drehknopf um eine Stufe nach links zu drehen. Was passiert?
~hint Mehr erfahren!
So funktioniert es:
- Die Variable enthält die aktuelle Temperatur. In diesem Programm beginnt die Temperatur bei 28 °C.
- Wenn du den Drehknopf drehst, ändert sich die Variable. Durch Drehen des Drehknopfs nach rechts wird die Temperatur erhöht, durch Drehen nach links wird sie verringert.
- Der Calliope mini überprüft ständig den Wert der Temperaturvariablen und zeigt ihn auf dem Bildschirm an.    
hint~

```block
let temperature = 28

fwdButtons.dial1.onRotated(fwdEnums.ClockwiseCounterclockwise.Clockwise, function () {
    temperature += 1
})

fwdButtons.dial1.onRotated(fwdEnums.ClockwiseCounterclockwise.Counterclockwise, function () {
    temperature += -1
})

basic.forever(function () {
    basic.showNumber(temperature)
})
```

## Ausprobieren Schritt 6

Drehe den Regler weiter, bis die Temperatur über 30 °C liegt.

Was fällt dir auf?
~hint Mehr erfahren!

-   Wenn die Temperatur über 30 °C liegt, leuchten die LEDs auf dem LED-Ring weiß.
-   Dies steht für die Korallenbleiche, die durch die Erwärmung des Ozeans verursacht wird.
    hint~

## Ausprobieren Schritt 7

Wir haben eine sogenannte **Bedingung** verwendet, um die Farbe unseres LED-Rings (auch bekannt als Koralle!) zu ändern.

Eine Bedingung ist eine Regel, die dem Calliope mini mitteilt, was zu tun ist, wenn bestimmte Bedingungen erfüllt sind. In diesem Modell ändert die Bedingung die Farbe des LED-Rings basierend auf der Temperatur.

## Ausprobieren Schritt 8

Kannst du die Bedingung im folgenden Code finden?
~hint Mehr erfahren!

- Bei Temperaturen über 30 °C bleicht die Koralle aus (die LED leuchtet weiß).
- Bei Temperaturen von 30 °C oder darunter bleibt die Koralle gesund (die LED leuchtet weiterhin rosa).
    hint~

```block
    if (temperature > 30) {
        fwdLights.ledRing1.setAllPixelsColor(0xffffff)
    } else {
        fwdLights.ledRing1.setAllPixelsColor(0xff0080)
    }
```

## Ausprobieren Schritt 9

Inwiefern ist dies ein gutes Modell für die Korallenbleiche im wirklichen Leben?
~hint Mehr erfahren!

Stärken:

- Dieses Modell zeigt deutlich, wie wärmeres Wasser zur Korallenbleiche führen kann.
- Es zeigt, dass bereits ein geringer Temperaturanstieg eine Korallenbleiche verursachen kann.
- Das Modell nutzt Farben auf hilfreiche Weise. In der Realität sind Korallen zunächst farbig, werden aber weiß, wenn sie bleichen – genau wie unser LED-Ring!
- In unserem Modell können Menschen die Temperatur des Ozeans beeinflussen, indem sie den Regler drehen. In der Realität können wir zwar keinen Regler drehen, aber wir können Maßnahmen wie die Reduzierung der Umweltverschmutzung ergreifen, um die Temperatur des Ozeans zu senken und Korallenriffe zu schützen.
    hint~

## Ausprobieren Schritt 10

Was sind einige Einschränkungen dieses Modells? Zeigt es wirklich alles, was in einem echten Korallenriff passiert?

~Hinweis Erzähl mir mehr!

- In diesem Modell tritt die Bleiche plötzlich auf. In Wirklichkeit verläuft die Korallenbleiche langsam über einen längeren Zeitraum, wenn die Wassertemperatur steigt.
- Das Modell zeigt nur Temperaturänderungen, aber in der Realität können auch Faktoren wie Umweltverschmutzung oder zu viel Sonnenlicht zur Korallenbleiche führen.
- Dieses Modell zeigt nicht, wie sich Korallen erholen und wieder gesund werden können.
- Das Modell zeigt nicht, wie sich die Korallenbleiche auf andere Tiere auswirkt, die im Riff leben.

Wählen eine dieser Einschränkungen aus. Wie könnten wir das Modell verbessern, um dieses Problem zu beheben? Welche Komponenten des Climate Action Kits würdest du hinzufügen?
hint~

## Herzlichen Glückwunsch! @showdialog

Du hast hast diese Aktivität abgeschlossen!

## Analyse @showdialog

Nenne zwei neue Dinge, die du heute gelernt hast.

Was ist eine Sache, über die du mehr erfahren möchtest?


## Fertig! @showdialog

Im nächsten Schritt kannst du auf die Schaltfläche `|Done|` klicken, um das Tutorial zu beenden.

## Fertig!

Du kannst auf die Schaltfläche `|Done|` klicken, um das Tutorial zu beenden.

Besuch auch mal calliope.cc, um weitere inspirierende Ideen und Projekte zu entdecken!