# Forward Education Wind Turbine - Sample Tutorial

```package
fwd-climate-action=github:calliope-edu/climate-action#v1.1.0
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

1. **Bauen** Den Prototypen konstruieren
2. **Code erstellen** Das Projekt zum Leben zu erwecken
3. **Ausprobieren** Herausfinden, ob der fertige Prototyp funktioniert
4. **Modifizieren** Verändere dein Projekt mit einer kleinen Programmieraufgabe

<img src="https://raw.githubusercontent.com/calliope-edu/climate-action-kit/add3c3f5d4b963f2cba276ba9760a9f8c463b77c/tutorial-assets/ms-windsample-render.webp" alt="Full sample wind tubine render" style="display: block; width: 60%; margin:auto;">

## Bauanleitung Schritt 1 @showdialog

![sbs1](https://raw.githubusercontent.com/calliope-edu/climate-action-kit/add3c3f5d4b963f2cba276ba9760a9f8c463b77c/tutorial-assets/ms-windsample-sbs01.webp)

## Bauanleitung Schritt 2 @showdialog

![sbs1](https://raw.githubusercontent.com/calliope-edu/climate-action-kit/add3c3f5d4b963f2cba276ba9760a9f8c463b77c/tutorial-assets/ms-windsample-sbs02.webp)

## Bauanleitung Schritt 3 @showdialog

![sbs1](https://raw.githubusercontent.com/calliope-edu/climate-action-kit/add3c3f5d4b963f2cba276ba9760a9f8c463b77c/tutorial-assets/ms-windsample-sbs03.webp)

## Bauanleitung Schritt 4 @showdialog

![sbs1](https://raw.githubusercontent.com/calliope-edu/climate-action-kit/add3c3f5d4b963f2cba276ba9760a9f8c463b77c/tutorial-assets/ms-windsample-sbs04.webp)

## Bauanleitung Schritt 5 @showdialog

![sbs1](https://raw.githubusercontent.com/calliope-edu/climate-action-kit/add3c3f5d4b963f2cba276ba9760a9f8c463b77c/tutorial-assets/ms-windsample-sbs05.webp)

## Bauanleitung Schritt 6 @showdialog

![sbs1](https://raw.githubusercontent.com/calliope-edu/climate-action-kit/add3c3f5d4b963f2cba276ba9760a9f8c463b77c/tutorial-assets/ms-windsample-sbs06.webp)

## Bauanleitung Schritt 7 @showdialog

![sbs1](https://raw.githubusercontent.com/calliope-edu/climate-action-kit/add3c3f5d4b963f2cba276ba9760a9f8c463b77c/tutorial-assets/ms-windsample-sbs07.webp)

## Bauanleitung Schritt 8 @showdialog

![sbs1](https://raw.githubusercontent.com/calliope-edu/climate-action-kit/add3c3f5d4b963f2cba276ba9760a9f8c463b77c/tutorial-assets/ms-windsample-sbs08.webp)

## Bauanleitung Schritt 9 @showdialog

![sbs1](https://raw.githubusercontent.com/calliope-edu/climate-action-kit/add3c3f5d4b963f2cba276ba9760a9f8c463b77c/tutorial-assets/ms-windsample-sbs09.webp)

## Bauanleitung Schritt 10 @showdialog

![sbs1](https://raw.githubusercontent.com/calliope-edu/climate-action-kit/add3c3f5d4b963f2cba276ba9760a9f8c463b77c/tutorial-assets/ms-windsample-sbs10.webp)

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

The Climate Action Kit lesson library allows students to scaffold their learning in three stages of projects: **Use, Modify, and Create.**

Now that we've built our wind turbine, we'll start by **using** sample code to see how it works.

As you go through the next steps:

-   **Use** the instructions at the top of the screen.
-   When you are ready for more information, click **'Tell Me More!'**
-   If you need help with the code, click the **lightbulb**!

<img src="https://raw.githubusercontent.com/calliope-edu/climate-action-kit/main/tutorial-assets/tellmore_hintbox_gif.webp" style="display: block; width: 80%; margin:auto;">

## Ausprobieren Schritt 1

The code in the workspace will make our wind turbine turn and stop.

## Ausprobieren Schritt 2

As you turn the dial to the **right**, watch what happens in the virtual simulator panel _and_ on your physical wind turbine.

~hint Tell Me More!

-   You can use the simulators on the left of the workspace to see what's happening to your Climate Action Kit in real time as your motor and dials turn!
-   When we turn the dial to the right, the motor should respond in the virtual simulator **and** the wind turbine!
-   This is what is called the **input** and **output** of the code:
    _ **Input** - turn the dial to the right
    _ **Output** - motor spins to the right
    hint~

## Ausprobieren Schritt 3

Look at your code. How do you think we can **stop** the motor from spinning? Try it!

~hint Tell Me More!

-   The motor will **stop** when you press down on the **dial**!
    hint~

## Ausprobieren Schritt 4

What do you think will happen when you turn the dial to the **left**? Try it now!

~hint Tell Me More!

-   Nothing happens! There is no code that tells the computer what to do when the dial is turned this direction.
    hint~

## Challenge Time! @showdialog

The Climate Action Kit lesson library allows students to **modify** their project using coding or build challenges!

Now that we have **used** code to create a wind turbine that turns **right** when we turn the dial **right**, we need to **modify** our code to make the wind turbine turn **both directions**.

## Modifizieren Schritt 1

In the workspace, there is an `||fwdSensors:on dial1 turned difference||` event we haven't used yet. How can you use this empty event to make the wind turbine turn **left** when we turn the dial to the **left**?

~hint Tell Me More!

-   The `||fwdSensors:on dial1 turned difference||` block is the block that is going to sense the new **input** (the dial turning **left**).
    hint~

```blocks
fwdButtons.dial1.onRotated(fwdEnums.ClockwiseCounterclockwise.Counterclockwise, function () {
})
```

## Modifizieren Schritt 2

Open the `||fwdMotors:Motors||` category and drag and drop `||fwdMotors:set leftServo to 50 %||` into the workspace.

On the sensor block, click the dropdown from set **leftServo** to set **middleServo**

~hint Tell Me More!

-   You can use up to **3 motors at a time** using the Climate Action Kit! We've built our wind turbine using the **middle** port (M), so we need to program our sensor using the **middle** servo.
-   The **motor** is the block that will respond with our new **output** (the motor spinning **left**).
    hint~

```block
 fwdBase.middleServo.setSpeed(50)
```

## Modifizieren Schritt 3

How can you combine the `||fwdSensors:on dial1 turned difference||` event and the `||fwdMotors:set middleServo to 50 %||` together to make the wind turbine turn **left** when the dial is turned **left**?

~hint Tell Me More!

-   Drag and drop the blue `||fwdMotors:set middleServo to 50 %||` block into the empty `||fwdSensors:on dial1 turned difference||` event.
-   Note: The motor block should now turn blue!
    hint~

```block
fwdButtons.dial1.onRotated(fwdEnums.ClockwiseCounterclockwise.Counterclockwise, function () {
    fwdBase.middleServo.setSpeed(50)
})
```

## Modifizieren Schritt 4

Click the `|Download|` button to download the code to your project.

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

How do you think that you could use the Climate Action Kit in your classroom?

What is one thing you want to learn more about?

## Fertig! @showdialog

Im nächsten Schritt kannst du auf die Schaltfläche `|Done|` klicken, um das Tutorial zu beenden.

## Fertig!

Du kannst auf die Schaltfläche `|Done|` klicken, um das Tutorial zu beenden.

Besuch auch mal die Webseite calliope.cc, um weitere inspirierende Ideen und Projekte zu entdecken!