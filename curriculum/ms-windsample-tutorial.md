# Forward Education Wind Turbine - Sample Tutorial

```package
fwd-climate-action=github:calliope-edu/climate-action-kit
datalogger=datalogger
```

```template
fwdButtons.touch1.onEvent(jacdac.ButtonEvent.Down, function () {
    fwdBase.middleServo.setSpeed(0)
})

fwdButtons.dial1.onRotated(fwdEnums.ClockwiseCounterclockwise.Clockwise, function () {
    fwdBase.middleServo.setSpeed(-50)
})

fwdButtons.dial1.onRotated(fwdEnums.ClockwiseCounterclockwise.Counterclockwise, function () {

})
```

## Aktivität 1: Erstelle dein Projekt @showdialog

Lasst uns eine automatisierte Windkraftanlage bauen. Wir werden dies in vier Schritten tun:

1. **Bauen:** Den Prototypen konstruieren
2. **Code erstellen:** Das Projekt zum Leben zu erwecken
3. **Ausprobieren:** Herausfinden, ob der fertige Prototyp funktioniert
4. **Modifizieren:** Verändere dein Projekt mit einer kleinen Programmieraufgabe

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

## Activity 2: Code erstellen @showdialog

Wir müssen unser Projekt mit dem Computer verbinden, damit es mit Code zum Leben erweckt wird!

Der Code enthält die Anweisungen, die unserem Calliope mini sagen, was er tun soll.

## Code Schritt 1 @showdialog

WICHTIG! Vergewissere sich, dass dein Climate Action Kit Breakout Board eingeschaltet und der Calliope mini an einem Computer angeschlossen ist.
<img src="https://raw.githubusercontent.com/calliope-edu/climate-action-kit/main/tutorial-assets/pluganim.webp" alt="Plug Calliope mini into USB port on computer" style="display: block; width: 40%; margin:auto;">

## Code Schritt 2 @showdialog

Klicke auf die drei Punkte neben der Schaltfläche '|Download|' und dann auf „Gerät verbinden“.
Befolge anschließend die Schritte zum Koppeln des Calliope mini.

<img src="https://raw.githubusercontent.com/calliope-edu/climate-action-kit/main/tutorial-assets/pairmicrobitGIF.webp"  alt="Pairing gif" style="display: block; width: 60%; margin:auto;">

## Code Schritt 3

Klicke anschließend auf die Schaltfläche `|Download|`, um den Code vom Projekt herunterzuladen.

## Aktivität 3: Ausprobieren @showdialog

Die Lektionsbibliothek des Climate Action Kit ermöglicht es, Lernen in drei Projektphasen zu strukturieren: **Verwenden, Modifizieren und Erstellen.**

Nachdem wir nun unsere Windkraftanlage gebaut haben, beginnen wir damit, den Beispielcode zu **verwenden**, um zu sehen, wie sie funktioniert.

Während du die nächsten Schritte durchgehst:

- **Verwende** die Anweisungen oben auf dem Bildschirm.
- Wenn du weitere Informationen benötigst, klicke auf **„Mehr erfahren!“** ().
- Wenn du Hilfe beim Code benötigst, klicke auf die **Glühbirne**!

<img src="https://raw.githubusercontent.com/calliope-edu/climate-action-kit/main/tutorial-assets/tellmore_hintbox_gif.webp" style="display: block; width: 80%; margin:auto;">

## Ausprobieren Schritt 1

Der Code im Arbeitsbereich sorgt dafür, dass sich unsere Windkraftanlage dreht und stoppt.
## Ausprobieren Schritt 2

Wenn du den Drehknopf nach **rechts** drehen, beobachten Sie, was im virtuellen Simulator-Panel _und_ an Ihrer physischen Windkraftanlage passiert.
~hint Mehr erfahren!

-   Mit den Simulatoren auf der linken Seite des Arbeitsbereichs kannst du in Echtzeit verfolgen, was mit dem Climate Action Kit passiert, wenn du den Motor und die Drehregler betätigst!
- Wenn wir den Drehregler nach rechts drehen, sollte der Motor im virtuellen Simulator **und** in der Windkraftanlage reagieren!
- Dies wird als **Eingabe** und **Ausgabe** des Codes bezeichnet:
    _ **Eingabe** – Drehknopf nach rechts drehen
    _ **Ausgabe** – Motor dreht sich nach rechts
    hint~

## Ausprobieren Schritt 3

Schau dir deinen Code an. Wie können wir deiner Meinung nach den Motor daran hindern, sich zu drehen? Probiere es aus!

~hint Mehr erfahren!

-   The motor will **stop** when you press down on the **dial**!
    hint~

## Ausprobieren Schritt 4

Was glaubst du, was passiert, wenn du den Regler nach **links** drehst? Probiere es jetzt aus!

~hint Mehr erfahren!

- Es passiert nichts! Es gibt keinen Code, der dem Computer mitteilt, was zu tun ist, wenn der Drehknopf in diese Richtung gedreht wird.
   hint~

## Challenge Time! @showdialog

Die Übungen des Climate Action Kit ermöglicht es, ein Projekt mithilfe von Programmier- oder Konstruktionsaufgaben zu **modifizieren**!

Nachdem wir nun mithilfe von Code eine Windkraftanlage erstellt haben, die sich **nach rechts** dreht, wenn wir den Drehknopf **nach rechts** bewegen, müssen wir unseren Code **modifizieren**, damit sich die Windkraftanlage **in beide Richtungen** dreht.

## Modifizieren Schritt 1

Im Arbeitsbereich gibt es ein Ereignis „||fwdSensors:on dial1 turned difference||“, das wir noch nicht verwendet haben. Wie kannst du dieses leere Ereignis verwenden, damit sich die Windkraftanlage nach **links** dreht, wenn wir den Drehknopf auch nach **links** drehen?

~hint Mehr erfahren!

-   Der Block „||fwdSensors:on dial1 turned difference||“ ist der Block, der die neue **Eingabe** (das Drehen des Drehknopfs nach **links**) erfasst.
    hint~

```blocks
fwdButtons.dial1.onRotated(fwdEnums.ClockwiseCounterclockwise.Counterclockwise, function () {
})
```

## Modifizieren Schritt 2

Öffne die Kategorie „||fwdMotors:Motors||“ und ziehe „||fwdMotors:set leftServo to 50 %||“ per Drag & Drop auf die Bühne.

Klicke im Sensorblock auf das Dropdown-Menü von „setze **linken Servo**“.
~hint Mehr erfahren!

- Mit dem Climate Action Kit kannst du bis zu **3 Motoren gleichzeitig** verwenden! Wir haben unsere Windkraftanlage mit dem **mittleren** Anschluss (M) gebaut, daher müssen wir unseren Sensor mit dem **mittleren** Servo programmieren.
- Der **Motor** ist der Block, der mit unserer neuen **Ausgabe** reagiert (der Motor dreht sich nach **links**).

    hint~

```block
 fwdBase.middleServo.setSpeed(50)
```

## Modifizieren Schritt 3

Wie kann man das Ereignis „||fwdSensors:on dial1 turned difference||“ und „||fwdMotors:set middleServo to 50 %||“ kombinieren, damit sich die Windkraftanlage **nach links** dreht, wenn der Drehknopf auch **nach links** gedreht wird?

~hint Mehr erfahren!

- Ziehe den blauen Block „||fwdMotors:set middleServo to 50 %||“ per Drag & Drop in das leere Ereignis „||fwdSensors:on dial1 turned difference||“.
- Hinweis: Der Motorblock sollte nun blau werden!
    hint~

```block
fwdButtons.dial1.onRotated(fwdEnums.ClockwiseCounterclockwise.Counterclockwise, function () {
    fwdBase.middleServo.setSpeed(50)
})
```

## Modifizieren Schritt 4

Klicke auf die Schaltfläche `|Download|`, um den Code in Ihr Projekt herunterzuladen.
```block
fwdButtons.touch1.onEvent(jacdac.ButtonEvent.Down, function () {
    fwdBase.middleServo.setSpeed(0)
})

fwdButtons.dial1.onRotated(fwdEnums.ClockwiseCounterclockwise.Clockwise, function () {
    fwdBase.middleServo.setSpeed(-50)
})

fwdButtons.dial1.onRotated(fwdEnums.ClockwiseCounterclockwise.Counterclockwise, function () {
    fwdBase.middleServo.setSpeed(50)
})
```

## Analyse @showdialog

Wie Kannst du das Climate Action Kit in deinem Unterricht einsetzen?

Über welches Thema möchtest du mehr erfahren?

## Fertig! @showdialog

Im nächsten Schritt kannst du auf die Schaltfläche `|Done|` klicken, um das Tutorial zu beenden.

## Fertig!

Du kannst auf die Schaltfläche `|Done|` klicken, um das Tutorial zu beenden.

Besuch auch mal calliope.cc, um weitere inspirierende Ideen und Projekte zu entdecken!