# Trübungsmessgeräte – Tutorial

```package
fwd-climate-action=github:Forward-Education/pxt-climate-action#v1.1.0
datalogger=datalogger
```

```template
input.onButtonPressed(Button.A, function () {
    basic.showNumber(fwdSensors.solar1.lightLevel())
})
fwdLights.ledRing1.setBrightness(10)
fwdLights.ledRing1.setAllPixelsColor(0xffffff)
```

## Trübungsmessgeräte @showdialog

Heute bauen wir unseren eigenen **NTU-Sensor**, um die Trübung von Wasserproben zu messen!

<img src="https://raw.githubusercontent.com/calliope-edu/climate-action-kit/main/tutorial-assets/ms-turbidity-render.webp" alt="Full turbidity meter render" style="display: block; width: 100%; margin:auto;">
Ein **NTU-Sensor** (Nephelometric Turbidity Unit) ist ein Sensor, der zur Messung der Trübung in Flüssigkeiten verwendet wird. Die Einheit NTU wird in der Wasseraufbereitung verwendet, um die Trübung zu messen.

## Schritt 1 @showdialog
Wir müssen unser Modell mit dem Computer verbinden, damit es mit Code zum Leben erweckt werden kann!

Der Code enthält die Anweisungen, die unserem Calliope mini sagen, was er tun soll.

WICHTIG! Vergewissere dich, dass dein Climate Action Kit Breakout Board eingeschaltet und dein Calliope mini an einem Computer angeschlossen ist.

<img src="https://raw.githubusercontent.com/calliope-edu/climate-action-kit/main/tutorial-assets/pluganim.webp" alt="Plug Calliope mini into USB port on computer" style="display: block; width: 40%; margin:auto;">

## Schritt 2 @showdialog

Klicke auf die drei Punkte neben der Schaltfläche `|Download|` und dann auf „Gerät verbinden“.
Befolge anschließend die Schritte zum Koppeln des Calliope mini.

<img src="https://raw.githubusercontent.com/calliope-edu/climate-action-kit/main/tutorial-assets/pairmicrobitGIF.webp"  alt="Pairing gif" style="display: block; width: 60%; margin:auto;">

## Schritt 3

Klicke anschließend auf die Schaltfläche `|Download|`, um den Code vom Projekt herunterzuladen.

## Schritt 4

Schaue dir dein physisches Projekt an. Kannst du die Hauptteile des NTU-Sensors identifizieren?


Denke daran:

-   **NTU-Sensoren** benötigen eine Lichtquelle und einen Lichtsensor.

-   Wir verwenden den **LED-Ring** als Lichtquelle und den **Sonnensensor** als Lichtsensor.

-   Der LED-Ring strahlt Licht direkt durch die Wasserprobe.

-   Der Sonnensensor wird senkrecht zum LED-Ring platziert, um das von den Schwebeteilchen in der Probe gestreute Licht aufzunehmen! Schaue dir den  den Hinweis an, um dir ein Bild davon zu machen.

hint~

![Light scatter in NTU sensors](https://raw.githubusercontent.com/calliope-edu/climate-action-kit/main/tutorial-assets/NTUsensor-cloudysample.png)

## Schritt 5

Schaue dir den Code im Arbeitsbereich an. Was glaubst du, wird dieser Code bewirken?
 
~hint Mehr erfahren!

-   Die beiden Blöcke `||fwdSensors:LED ring||` in `||basic:on start||` weisen den Calliope mini an, die Lichtquelle unseres NTU-Sensors auf volle Helligkeit zu schalten.

- `||input:on button A pressed||` Der vom Sonnensensor erfasste Wert wird auf den LEDs des Calliope mini angezeigt. Auf diese Weise können wir unseren Messwert ablesen!

hint~

```blocks
fwdLights.ledRing1.setBrightness(10)
fwdLights.ledRing1.setAllPixelsColor(0xffffff)
input.onButtonPressed(Button.A, function () {
    basic.showNumber(fwdSensors.solar1.lightLevel())
})
```

## Schritt 6

Stelle die vorbereiteten Wasserproben zur Messung bereit.

Denke daran, dass unsere Probe mit geringerer Trübung Leitungswasser sein sollte, während die zweite Probe mit höherer Trübung Leitungswasser mit einem Esslöffel Backpulver sein soll.

## Schritt 7

Platziere die Probe mit geringer Trübung zwischen dem LED-Ring und dem Sonnensensor, wie in der Glühbirnen-Anleitung gezeigt. Stelle sicher, dass die Wasserprobe stabil ist und nicht verschüttet werden kann.

![Low turbidity sample](https://raw.githubusercontent.com/calliope-edu/climate-action-kit/main/tutorial-assets/ms-turbidity-water-render.webp)

## Schritt 8

Drücke A. Wie lautete der Messwert für diese Probe? Notiere ihn.

## Schritt 9

Platziere die Probe mit hoher Trübung zwischen dem LED-Ring und dem Sonnensensor, wie in der Glühbirnen-Anleitung gezeigt. Stelle sicher, dass die Wasserprobe stabil steht.

Wie wird sich der Messwert dieser Probe deiner Meinung nach vom ersten unterscheiden? Warum?
![High turbidity sample](https://raw.githubusercontent.com/calliope-edu/climate-action-kit/main/tutorial-assets/ms-turbidity-dirty-render.webp)

## Schritt 10

Drücke A. Notiere den Messwert. War deine Vorhersage richtig?

## Schritt 11

Analysieren deine gemessenen Daten:

1. Welche Probe wies einen höheren Trübungswert auf?
2. Was sagt der Unterschied in den Messwerten über die Klarheit der beiden Proben aus?
3. Was sagt dieser Unterschied über die Partikelmenge in jeder Probe aus?


## Herzlichen Glückwunsch! @showdialog

Du hast hast diese Aktivität abgeschlossen!

## Analyse @showdialog

Bevor wir zum Schluss kommen:

- Warum ist es wichtig, bei der Messung der Trübung mehr als eine Wasserprobe zu testen?
- In welchem Zusammenhang steht die Menge des gestreuten Lichts mit der Trübung einer Wasserprobe?
- In welchen Situationen im Alltag ist es wichtig, die Trübung zu messen?
- Wenn du in einer lokalen Wasserprobe einen hohen Trübungswert festgestellt hast, was könnten mögliche Ursachen für die Partikel sein, die die Trübung verursachen?

## Fertig!

Du kannst auf die Schaltfläche `|Done|` klicken, um das Tutorial zu beenden.

Besuch auch mal calliope.cc, um weitere inspirierende Ideen und Projekte zu entdecken!
