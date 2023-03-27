# LA-1500
# Projekt-Dokumentation


Gruppe-Lilac | Hitz, Meister, Angelov, Lai, Schneider

| Datum | Version | Zusammenfassung                                              |
| ----- | ------- | ------------------------------------------------------------ |
| 21.02.2023      | 0.0.1   | Heute haben wir die User Stories, ein Pap und ein Use Case Driagramm erstellt. |
| 28.02.2023      | 0.0.2     | Heute haben wir die User Stories erweitert, den Plan erstellt und Unity installiert.                                |
| 07.03.2023      | 0.0.3   | Heute haben wir die Basics unseres Speils programmiert, wie die Objekte und das Springen       |
| 14.03.2023      | 0.0.4   | Heute haben wir die Grundanforderungen des Spiels fertig PRogrammiert.      |
| 15.03.2023      | 0.0.5   | Heute haben wir die Kann-Anforderungen weiterprogrammiert und die Präsentation für das Projekt erstellt.    |

## 1 Informieren

### 1.1 Ihr Projekt

Wir programmieren eine Nachstellung des Chrome Dino run game.

Unser Ziel ist es ein Spiel zu coden welches ähnlich ist, wie das Chrome Dino run game. Das Spiel ist zweidimensional und besteht aus einem Charakter welcher rennt und dabei Hindernissen ausweicht. Das macht man indem man springt. Während einem Run erhöht sich die Geschwindigkeit immer weiter bis man in ein Hindernis rennt. Wir orientieren uns nur am Spielprinzip. Die Figur und die anderen Elemente designen wir selber. Wir implementieren dieses Spiel mit Unity.
Wir wollen in diesem Projekt lernen wie man Elemente wie zum Beispiel eine Figur im Spiel herumbewegen kann.

### 1.2 User Stories

| US-№ | Verbindlichkeit | Typ  | Beschreibung                       |
| ---- | --------------- | ---- | ---------------------------------- |
| 1    | kann               | funktional     | Als User möchte ich, ein Startbildschirm nach Programmstart sehen, damit ich weiss, dass ich im Spiel bin. |
| 2  |    muss             |  funktional    |  Als User möchte ich ein Startbutton, damit ich das Spiel starten kann.            |
| 3  |      muss           |  funktional    | Als User möchte ich, dass meine Figur springen und doppelt Springen kann, damit ich den Objekten ausweichen kann.           |
| 4  |   muss              |  funktional    |  Als User möchte ich, dass Verschiedengrosse Objekte zum drüber Springen auf mich zukommen, damit das Spiel spannender ist.            |
| 5  |     muss            | funktional     | Als User möchte ich, dass Game Over ist, wenn ich ein Objekt berühre und kein Extraleben mehr habe, damit ich weiss, dass das Spiel beendet wurde.         |
| 6 |  kann               | funktional     |  Als User möchte ich eine Highscoreanzeige nach Game Over, damit ich weiss, wie hoch mein Score in diesem Run war.                       |
| 7  |   kann              |  Qualitativ    |  Als User möchte ich die Figur wechseln können im Startbildschirm, damit ich mehr Abwechslung bei meiner Figur habe.               |
| 8 |   kann              |  funktional    |   Als User möchte ich das Pausenmenu öffnen können, während einem Run, damit ich den Run temporär Unterbrechen kann.                  |
| 9 |  kann               | funktional     | Als User möchte ich eine Mapauswahl vor dem Start eines Runs haben, damit ich mehr Abwechslung im Spiel habe.             |
| 10  |   muss              |   funktional   | Als User möchte ich einen Button, um das Spiel verlassen zu können, damit ich das Spiel beenden kann.              |
| 11 |  muss               |  funktional    | Als User möchte ich Getränke aufsammeln können, welche einen zufälligen Effekt geben, damit das Spielerlebnis interessanter ist.    |
| 12 |   muss              |   funktional   |  Als User möchte ich, wenn ich das  Jump boost Effekt Getränk einsammle, dass meine Sprünge doppelt so hoch sind, damit ich den Objekten besser ausweichen kann.              |
| 13  |   muss             |  funktional    |  Als User möchte ich, wenn ich das Unsterblichkeit Effekt Getränk einsammle, dass ich Immun gegen alle Objekte bin, damit ich so länger überleben kann.   |
| 14  |     muss            |  funktional    | Als User möchte ich, wenn ich durch einen Ring durchlaufe, dass ich beginne zu fliegen und durch verschiedene weitere Ringe durchfliegen muss, damit ich ein Extra life bekommen kann.   | 
| 15  |    muss             |  funktional    | Als User möchte ich, wenn ich das Speed Boost Effekt Getränk einsammle, dass meine Figur viel schneller rennt,  damit das Spiel für kurze Zeit schwieriger wird. |
| 16  |   muss              |  funktional    | Als User möchte ich, dass alle Getränke ausser Extra life 5 sekunden dauern, damit ich den Effekt nicht das ganze Spiel habe.   |
| 17  |     kann            |  funktional    | Als User möchte ich einen Timer haben, welcher mir die verbleibende Zeit des Effekts angibt, damit ich weiss wie lange der Effekt noch anhält.  |
| 18  |    kann             |  funktional    |  Als User möchte ich einen Explosions Animation haben wenn ich mit dem Immun Effekt durch Objekte renne.  |   
| 19  |    muss            |  funktional    |  Als User möchte ich, wenn ich beim Extra life den Boden oder die Decke berühre, dass ich sterbe, damit das Spiel nicht zu einfach ist | 
| 20  |    muss             |  funktional    |  Als User möchte ich, wenn ich in das Reverse Item laufe, dass die Ganze Welt gedreht wird, damit es noch mehr Abwechslung im Spiel gibt. |




### 1.3 Testfälle

| TC-№ | Ausgangslage | Eingabe | Erwartete Ausgabe |
| ---- | ------------ | ------- | ----------------- |
| 1.1  |  Programm gestartet            |    -     |   Startbildschirm angezeigt         |
| 2.1 |  im Startbildschirm            |   Startbutton gedrückt     |       Spiel startet            |
| 3.1 |  im Spiel            |    Spacebar gedrückt     |      Figur springt             |
| 3.2 |  im Sprung            |    Spacebar gedrückt     |        zweiter Sprung           |
| 4.1  |  im Spiel            |    -     |        Objekt zum bewegt sich auf die Figur zu           |
| 5.1 |   Im Spiel mit Objekt kolidiert           |    -     |   Game over           |
| 6.1  |   Game over           |     -    |    Highscore wird angezeigt               |
| 7.1  |   im Startbildschirm           |    auf Figur wechseln gedrückt    |    Figurenanzeige wird angezeigt              |
| 7.2 |     in Figurenanzeige         |    auf Figur x gedrückt     |   Figur x als Spielfigur ausgewählt                |
| 8.1 |   im Spiel           |    Esc oder Pause-button gedrückt     |        Pausenmenu angezeigt           |
| 8.2  |  im Pausenmenu       |  Quit-Button gedrückt       |      Zum Startbildschirm             |
| 8.3  |  im Pausenmenu            |    Resume-Button gedrückt     |   Zurück zum Spiel                |
| 9.1 |   Im Startbildschirm           |    Mapauswahl-Button gedrückt     |       Mapauswahl angezeigt            |
| 9.2  |  In Mapauswahl            |   Map x ausgewählt      |   Map x für den nächsten Spieldurchlauf                |
| 10.1 | Im Startbildschirm             |  QUIT GAME Button gedrückt       |    Programm wird geschlossen               |
| 11.1  | Im Spiel             |   Figur mit Getränk x kollidiert     |   Figur erhält Effekt x                |
| 12.1  | Mit Jumpboost Getränk kollidiert             |    -     |   Sprungkraft verdoppelt sich                |
| 13.1  | Mit Unsterblichkeitsgetränk kollidiert         |    Kollision mit Objekt    |     Objekt verschwindet (kein Game over)           |
| 14.1  | Mit Extra-Life Getränk kollidiert             |    Kollision mit Objekt     |         Objekt verschwindet (ein Mal)          |


### 1.4 Diagramme

![Use Case3](https://user-images.githubusercontent.com/110893594/223396164-56e99d7a-37c9-4df0-b84c-3fac25f2dc5a.png)

![Hauptprogramm 1](https://user-images.githubusercontent.com/112430127/224925251-b8248ddc-687b-49c4-97d2-8265cb970278.png)


## 2 Planen

| AP-№ | Frist | Zuständig | Beschreibung | geplante Zeit |
| ---- | ----- | --------- | ------------ | ------------- |
| 1.A  | 14.03.2023        |  Angelov            |Startbildschirm            |30'
| 2.A  | 14.03.2023         | Angelov          | Startbutton             | 30'              |
| 3.A  | 14.03.2023         | Meister          | Springen Figur             | 45'              |
| 4.A  |14.03.2023          | Hitz          | Hindernisse             |2*45'           |
| 5.A  | 14.03.2023         |  Lai         | Spielende            | 30'              |
| 6.A  |21.03.2023          |  Schneider         | Highscoreanzeige             | 30'              |
| 7.A  |21.03.2023          |  Schneider         | Wechsel der Figur             | 2*45              |
| 8.A  |21.03.2023          | Hitz          | Pausenmenu             | 30'              |
| 9.A  |21.03.2023          | Hitz        | Mapauswahl             | 3*45              |
| 10.A  |14.03.2023         | Angelov          | Button Spielverlass             | 30'              |
| 11.A  |14.03.2023         | Lai          | Getränke aufsammeln            | 45'              |
| 12.A  |14.03.2023         | Hitz          | Jump boost          | 3*45'              |
| 13.A  |14.03.2023         | Hitz          | Unsterblichkeit           | 45'              |
| 14.A  |14.03.2023         | Meister          | Extra life           | 3*45'              |
| 15.A  |14.03.2023         | Angelov          | Speed Boost            | 20'              |
| 16.A  |14.03.2023         | Lai          | Dauer der Getränke            | 30'              |
| 17.A  |14.03.2023         | Lai          | Timer vom Effekt            | 20'              |
| 18.A  |21.03.2023         | Schneider          | Explosions Animation bei Immunität           | 45'              |
| 19.A  |14.03.2023         | Schneider         | Sterben Berührung Boden / Decke bei Extra Leben          | 30'              |
| 20.A  |14.03.2023         | Meister          | Reverse Item        | 3*45'              | 

## 3 Entscheiden

Wir haben uns entschieden mehr Potions zu machen, damit das Spiel nicht so langweilig ist.

## 4 Realisieren

| AP-№ | Datum | Zuständig | geplante Zeit | tatsächliche Zeit |
| ---- | ----- | --------- | ------------- | ----------------- |
| 1.A  |07.03.2023      | Angelov      |  30'           | 45'        |
| 1.A  |14.03.2023      | Angelov      |  30'           | 2*45'        |
| 2.A  |14.03      | Angelov     |  30'            | 45*        |
| 3.A  |07.03.2022   | Justus      | 45'              | 2*45'       |
| 4.A  |07.03.2022   | Hitz      | 45'              | 3*45       |
| 5.A  |21.03.2023   |Lai       | 30'              | 45'       |
| 6.A  |-   |-       |-               |-        |
| 7.A  |-   |-       |-               |-        |
| 8.A  |21.03.2023   | Hitz      | 30'              |45'        |
| 9.A  |-   |-       |-               |-        |
| 10.A  |21.03.2023   |Angelov      | 30'              |45'        |
| 11.A  | 07.03.2023  | Lai   | 45'          | 2*45'        |
| 12.A  |21.03.2023   | Hitz     | 3*45'             |4*45'      |
| 13.A  |21.03.2023   | Hitz     | 45'              |         |
| 14.A  |21.03.2023   | Meister     | 3*45'              | 3*45'   |
| 15.A  |21.03.2023   | Angelov     | 20'              | 30'       |
| 16.A  |21.03.2023   | Lai     | 30'               | 30'      |
| 17.A  |21.03.2023   | Lai     | 20'              | 30'       |
| 18.A  |-  | -   |-               |-         |
| 19.A  |-  |-       |-               |-         |
| 20.A  |21.03.2023 |Meister        |  3*45            | 3*45'    |

## 5 Kontrollieren

### 5.1 Testprotokoll

| TC-№ | Datum | Resultat | Tester |
| ---- | ----- | -------- | ------ |
| 1.1  |       |          |        |
| ...  |       |          |        |

✍️ Vergessen Sie nicht, ein Fazit hinzuzufügen, welches das Test-Ergebnis einordnet.

### 5.2 Exploratives Testen

| BR-№ | Ausgangslage | Eingabe | Erwartete Ausgabe | Tatsächliche Ausgabe |
| ---- | ------------ | ------- | ----------------- | -------------------- |
| I    |              |         |                   |                      |
| ...  |              |         |                   |                      |

✍️ Verwenden Sie römische Ziffern für Ihre Bug Reports, also I, II, III, IV etc.

## 6 Auswerten

✍️ Fügen Sie hier eine Verknüpfung zu Ihrem Lern-Bericht ein.
