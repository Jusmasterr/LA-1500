# LA-1500
# Projekt-Dokumentation


Gruppe-Lilac | Hitz, Meister, Angelov, Lai, Schneider

| Datum | Version | Zusammenfassung                                              |
| ----- | ------- | ------------------------------------------------------------ |
| 21.02.2023      | 0.0.1   | Heute haben wir die User Stories, ein Pap und ein Use Case Driagramm erstellt. |
| 28.02.2023      | 0.0.2     | Heute haben wir die User Stories erweitert, den Plan erstellt und Unity installiert.                                                            |
|       | 1.0.0   |                                                              |

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

![Use-Case Nr 3 drawio](https://user-images.githubusercontent.com/110893594/221805585-0448406b-4893-4fca-9dfe-a177ebdbb0f5.png)

![Projekt](https://user-images.githubusercontent.com/112430127/221799847-37dea31e-d0e2-4c67-bfaf-5c0a956a12c5.png)

## 2 Planen

| AP-№ | Frist | Zuständig | Beschreibung | geplante Zeit |
| ---- | ----- | --------- | ------------ | ------------- |
| 1.A  | 07.03.2023        |  Hitz            |Startbildschirm            |30'
| 2.A  | 07.03.2023         | Angelov          | Startbutton             | 30'              |
| 3.A  | 07.03.2023         | Meister          | Springen Figur             | 45'              |
| 4.A  |07.03.2023          | Hitz          | Hindernisse             |2*45'           |
| 5.A  | 07.03.2023         |  Lai         | Spielende            | 30'              |
| 6.A  |07.03.2023          |  Angelov         | Highscoreanzeige             | 30'              |
| 7.A  |07.03.2023          |  Hitz         | Wechsel der Figur             | 2*45              |
| 8.A  |07.03.2023          | Schneider          | Pausenmenu             | 30'              |
| 9.A  |07.03.2023          |  Hitz        | Mapauswahl             | 3*45              |
| 10.A  |07.03.2023         | Schneider          | Button Spielverlass             | 30'              |
| 11.A  |07.03.2023         | Meister          | Getränke aufsammeln            | 45'              |
| 12.A  |07.03.2023         | Hitz          | Jump boost          | 3*45'              |
| 13.A  |07.03.2023         | Schneider          | Unsterblichkeit           | 45'              |
| 14.A  |07.03.2023         | Meister          | Extra life           | 3*45'              |
| 15.A  |07.03.2023         | Angelov          | Speed Boost            | 20'              |
| 16.A  |07.03.2023         | Lai          | Dauer der Getränke            | 30'              |
| 17.A  |07.03.2023         | Lai          | Timer vom Effekt            | 20'              |
| 18.A  |07.03.2023         | Meister          | Explosions Animation bei Immunität           | 45'              |
| 19.A  |07.03.2023         | Schneider         | Sterben Brührung Boden / Decke bei Extra Leben          | 30'              |
| 20.A  |07.03.2023         | Meister          | Reverse Item        | 3*45'              |

Total: 

✍️ Die Nummer hat das Format `N.m`, wobei `N` die Nummer der User Story ist, auf die sich das Arbeitspaket bezieht, und `m` von `A` an nach oben buchstabiert. Beispiel: Das dritte Arbeitspaket, das die zweite User Story betrifft, hat also die Nummer `2.C`.

✍️ Ein Arbeitspaket sollte etwa 45' für eine Person in Anspruch nehmen. Die totale Anzahl Arbeitspakete sollte etwa Folgendem entsprechen: `Anzahl R-Sitzungen` ╳ `Anzahl Gruppenmitglieder` ╳ `4`. Wenn Sie also zu dritt an einem Projekt arbeiten, für welches zwei R-Sitzungen geplant sind, sollten Sie auf `2` ╳ `3` ╳`4` = `24` Arbeitspakete kommen. Sollten Sie merken, dass Sie hier nicht genügend Arbeitspakte haben, denken Sie sich weitere "Kann"-User Stories für Kapitel 1.2 aus.

## 3 Entscheiden

Wir haben uns entschieden mehr Potions zu machen, damit das Spiel nicht so langweilig ist.

## 4 Realisieren

| AP-№ | Datum | Zuständig | geplante Zeit | tatsächliche Zeit |
| ---- | ----- | --------- | ------------- | ----------------- |
| 1.A  |       |           |               |                   |
| ...  |       |           |               |                   |

✍️ Tragen Sie jedes Mal, wenn Sie ein Arbeitspaket abschließen, hier ein, wie lang Sie effektiv dafür hatten.

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
