# Städtische Wärmeinseln - Tutorial

```package
fwd-climate-action-kit=github:calliope-edu/climate-action-kit
datalogger=datalogger
v3
```

```template
input.onLogoEvent(TouchButtonEvent.Pressed, function () {
    datalogger.deleteLog()
})
datalogger.setColumnTitles("Temperatur")
loops.everyInterval(60000, function () {
    datalogger.log(datalogger.createCV("Temperatur", input.temperature()))
})
basic.forever(function () {
    basic.showNumber(input.temperature())
})
```

## Städtische Wärmeinseln - Tutorial @showdialog

Heute werden wir vergleichen, wie schnell sich eine feuchte, helle Modell-Stadt und eine trockene, dunkle Modell-Stadt erwärmen.

Wir benutzen den Temperatursensor vom Calliope mini, um Daten zu sammeln und herauszufinden, wie Farben und Feuchtigkeit die Temperatur in der Stadt beeinflussen. In Städten kann ein Wärmeinsel-Effekt entstehen, weil Gebäude und Straßen Wärme stärker aufnehmen und speichern (absorbieren) und dadurch die Umgebung wärmer wird.

<p float="middle">
  <img src="https://raw.githubusercontent.com/calliope-edu/climate-action-kit/main/tutorial-assets/ms-heatislands-comparison.webp" alt="Base model city render" width="100%"/>
</p>

## Bauanleitung Schritt 1 @showdialog

![sbs1](https://raw.githubusercontent.com/calliope-edu/climate-action-kit/main/tutorial-assets/ms-heatislands-sbs01.webp)

## Bauanleitung Schritt 2 @showdialog

![sbs1](https://raw.githubusercontent.com/calliope-edu/climate-action-kit/main/tutorial-assets/ms-heatislands-sbs02.webp)

## Bauanleitung Schritt 3 @showdialog

![sbs1](https://raw.githubusercontent.com/calliope-edu/climate-action-kit/main/tutorial-assets/ms-heatislands-sbs03.webp)

## Bauanleitung Schritt 4 @showdialog

![sbs1](https://raw.githubusercontent.com/calliope-edu/climate-action-kit/main/tutorial-assets/ms-heatislands-sbs04.webp)

## Bauanleitung Schritt 5 @showdialog

![sbs1](https://raw.githubusercontent.com/calliope-edu/climate-action-kit/main/tutorial-assets/ms-heatislands-sbs05.webp)

## Bauanleitung Schritt 6 @showdialog

![sbs1](https://raw.githubusercontent.com/calliope-edu/climate-action-kit/main/tutorial-assets/ms-heatislands-sbs06.webp)

## Bauanleitung Schritt 7 @showdialog

![sbs1](https://raw.githubusercontent.com/calliope-edu/climate-action-kit/main/tutorial-assets/ms-heatislands-sbs07.webp)

## Bauanleitung Schritt 8 @showdialog

![sbs1](https://raw.githubusercontent.com/calliope-edu/climate-action-kit/main/tutorial-assets/ms-heatislands-sbs08.webp)

## Fertig! @showdialog

![sbs1](https://raw.githubusercontent.com/calliope-edu/climate-action-kit/main/tutorial-assets/ms-heatislands-sbs09.webp)

## Modell-Stadt 1 @showdialog

![sbs1](https://raw.githubusercontent.com/calliope-edu/climate-action-kit/main/tutorial-assets/ms-heatislands-sbs10.webp)

Bedecke die erste Modell-Stadt mit feuchtem, weißem Papier, um reflektierende Baumaterialien und Dachgärten nachzuahmen. Du kannst dafür auch ausgewrungene Papiertücher verwenden.

## Modell-Stadt 2 @showdialog

![sbs1](https://raw.githubusercontent.com/calliope-edu/climate-action-kit/main/tutorial-assets/ms-heatislands-sbs11.webp)

Bedecke die zweite Modell-Stadt mit trockenem, schwarzem Papier, um typische dunkle Baumaterialien darzustellen.

## Weitere Modelle  @showdialog

![sbs1](https://raw.githubusercontent.com/calliope-edu/climate-action-kit/main/tutorial-assets/ms-heatislands-sbs12.webp)

Du kannst auch weitere Modelle bauen, um zu testen, wie Faktoren neben Farbe und Feuchtigkeit den Wärmeinsel-Effekt beeinflussen.

## Weitere Modelle @showdialog

![sbs1](https://raw.githubusercontent.com/calliope-edu/climate-action-kit/main/tutorial-assets/ms-heatislands-sbs13.webp)

## Aktivität 1: Code erstellen @showdialog

Wir müssen unser Modell mit dem Computer verbinden, damit es mit Code zum Leben erweckt werden kann!

Der Code enthält die Anweisungen, die unserem Calliope mini sagen, was er tun soll.

## Schritt 1 @showdialog

WICHTIG! Vergewissere dich, dass dein Climate Action Kit Breakout Board eingeschaltet und dein Calliope mini an einem Computer angeschlossen ist.

<img src="https://raw.githubusercontent.com/calliope-edu/climate-action-kit/main/tutorial-assets/pluganim.webp" alt="Plug Calliope mini into USB port on computer" style="display: block; width: 40%; margin:auto;">

## Schritt 2 @showdialog

Klicke auf die drei Punkte neben der Schaltfläche `|Download|` und dann auf „Gerät verbinden“.
Befolge anschließend die Schritte zum Koppeln des Calliope mini.

<img src="https://raw.githubusercontent.com/calliope-edu/climate-action-kit/main/tutorial-assets/pairmicrobitGIF.webp"  alt="Pairing gif" style="display: block; width: 60%; margin:auto;">

## Schritt 3

Klicke anschließend auf die Schaltfläche `|Download|`, um den Code vom Projekt herunterzuladen.

## Schritt 4

Schau dir den Code im Arbeitsbereich an. Was glaubst du, was dieser Code macht?

~hint Mehr erfahren!

-   Wir benutzen die [Datalogger Erweiterung](https://makecode.calliope.cc/reference/datalogger$), um Daten vom [Temperatursensor](https://calliope.cc/calliope-mini/uebersicht#temperatur) des Calliope mini zu messen und zu speichern.
-   Alle 60.000 Millisekunden (60 Sekunden oder 1 Minute) misst der Calliope mini die Temperatur und speichert sie im Datenlog.
-   Die `||basic:dauerhaft|` Schleife sorgt dafür, dass der Calliope mini die aktuelle Temperatur immer auf der LED-Matrix anzeigt.
-   Der Block `||input:wenn Logo gedrückt|` löscht alle zuvor gespeicherten Daten, wenn du das Logo auf der Rückseite vom Calliope mini drückst.

hint~

```block
loops.everyInterval(60000, function () {
    datalogger.log(datalogger.createCV("Temperatur", input.temperature()))
})
basic.forever(function () {
    basic.showNumber(input.temperature())
})
input.onLogoEvent(TouchButtonEvent.Pressed, function () {
    datalogger.deleteLog()
})
```

## Schritt 5

Es ist Zeit, das Experiment vorzubereiten!

Trenne den Calliope mini vom Computer.
Stelle deine erste Modell-Stadt unter deine gewählte Lichtquelle (z. B. Lampe, Fensterbank, draußen).
Positioniere deine Stadt so, dass sie direktes Licht bekommt.

## Schritt 6

Verbinde den Calliope mini wieder mit dem Computer oder einer anderen Stromquelle.
Drücke das Logo vom Calliope mini, um alte Daten zu löschen. Lass dann den Calliope mini für eine festgelegte Zeit (z.B. 2 Stunden) die Temperatur messen.

## Schritt 7

Lade nach dem Experiment deine Daten herunter, indem du den Calliope mini wieder an den Computer anschließt und [diesen Anweisungen](https://calliope.cc/schulen/fortbildungen/datenverarbeitung) folgst.

## Schritt 8

Wiederhole die letzten Schritte mit der zweiten Modell-Stadt.
Achte darauf, deine erste Messreihe vorher separat zu speichern und dass das Modell denselben Abstand zur Lichtquelle hat wie zuvor.

## Schritt 9

Analysiere deine Daten\*:

1. Vergleiche die Temperaturdaten vom feuchten, hellen Modell und vom trockenen, dunklen Modell.
2. Welche Unterschiede siehst du bei den Temperaturmessungen?
3. Wie hoch war die Starttemperatur jedes Modells?
4. Wie schnell hat sich jedes Modell erwärmt?
5. Welche Höchsttemperatur hat jedes Modell erreicht?
6. Kannst du diese Unterschiede erklären?

\*[Oder schaue dir unsere Beispieldaten an](https://docs.google.com/spreadsheets/d/1HPbwILmBtJYUxIrBu_gQfZHdcS_uosqb3iE6Cr536gk/edit?usp=share_link)

## Reflexion

Bevor wir fertig sind:

-   Warum ist es wichtig, die Daten von zwei verschiedenen Modellen in diesem Experiment zu vergleichen?
-   Was zeigt uns dieses Experiment darüber, wie Farbe und Feuchtigkeit die Erwärmung von Städten beeinflussen?
-   Welche anderen Faktoren könnten die Temperatur beeinflussen, die wir in unseren Modellen _nicht_ berücksichtigt haben?
-   Wie können Städte diese Informationen nutzen, um kühlere und nachhaltigere städtische Räume zu gestalten?

## Fertig!

Du kannst auf die Schaltfläche `|Done|` klicken, um das Tutorial zu beenden.

Auf der Internetseite **calliope.cc** findest du weitere inspirierende Ideen und Projekte!