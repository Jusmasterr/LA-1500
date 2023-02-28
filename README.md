# LA-1500
# Projekt-Dokumentation


Gruppe-Lilac | Hitz, Meister, Angelov, Lai, Schneider

| Datum | Version | Zusammenfassung                                              |
| ----- | ------- | ------------------------------------------------------------ |
| 21.02.2023      | 0.0.1   | Heute haben wir die User Stories, ein Pap und ein Use Case Driagramm erstellt. |
|       | ...     |                                                              |
|       | 1.0.0   |                                                              |

## 1 Informieren

### 1.1 Ihr Projekt

Wir programmieren eine Nachstellung des Chrome Dino run game.

Unser Ziel ist es ein Spiel zu coden welches möglichst gleich ist wie das Chrome Dino run game. Das Spiel ist zweidimensional und besteht aus einem Charakter welcher rennt und dabei Hindernissen ausweicht. Das macht man indem man sich entweder duckt oder springt. Während einem Run erhöht sich die Geschwindigkeit immer weiter bis man in ein Hindernis rennt. Wir orientieren uns nur am Spielprinzip. Die Figur und die anderen Elemente designen wir selber. Wir implementieren dieses Spiel mit C# WIN Forms.
Wir wollen in diesem Projekt lernen wie man Elemente wie zum Beispiel eine Picture Box im Form herumbewegen kann.

### 1.2 User Stories

| US-№ | Verbindlichkeit | Typ  | Beschreibung                       |
| ---- | --------------- | ---- | ---------------------------------- |
| 1    | kann               | funktional     | Startbildschirm nach Programmstart. |
| 2  |    muss             |  funktional    |    Startbutton um das Spiel zu starten.             |
| 3  |      muss           |  funktional    |  Figur kann springen und doppelt Springen.          |
| 4  |   muss              |  funktional    |  Verschiedengrosse Objekte zum drüberspringen kommen auf die Figur zu.              |
| 5  |     muss            | funktional     |    Game over wenn ein Objekt berührt wird.        |
| 6 |  kann               | funktional     |     Highscoreanzeige nach Game over                      |
| 7  |   kann              |  funktional    |        Figur wechseln im Startbildschirm                |
| 8 |   kann              |  funktional    |   Pausenmenu während einem Run                   |
| 9 |  kann               | funktional     |    Mapauswahl vor dem Start eines Runs            |
| 10  |   kann              |   funktional   | Button um das Spiel verlassen                |
| 11 |  kann               |  funktional    |   Aufnehmbare Getränke welche einen zfäligen Effekt geben                               |
| 12 |   kann              |   funktional   |   Jump boost Effekt (erhöht die Sprünge)                              |
| 13  |   kann              |  funktional    |  Unsterbbarkeit Effekt (macht Figur unsterblich)                             |
| 14  |     kann            |  funktional    |  Extra life Effekt (Gibt der Figur ein zusätzliches Leben)                             |
| 15  |    kann             |  funktional    |  Speed boost Effekt (erhöht die Geschwindigkeit der Figur drastisch)                                  |





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
| 15.1  | Mit Speed-Boost Getränk kollidiert             |    -     |         Geschwindigkeit wird erhöht         |


### 1.4 Diagramme

![JumpRun2](https://user-images.githubusercontent.com/110893594/220322372-9c95d3dc-fbd3-4c79-9731-65979f5f26a8.png)

![Pap LA_1500](https://user-images.githubusercontent.com/110893098/220320898-288013e3-080c-4a50-ac8a-669ab5964c91.png)

## 2 Planen

| AP-№ | Frist | Zuständig | Beschreibung | geplante Zeit |
| ---- | ----- | --------- | ------------ | ------------- |
| 1.A  |       |           |              |               |
| ...  |       |           |              |               |

Total: 

✍️ Die Nummer hat das Format `N.m`, wobei `N` die Nummer der User Story ist, auf die sich das Arbeitspaket bezieht, und `m` von `A` an nach oben buchstabiert. Beispiel: Das dritte Arbeitspaket, das die zweite User Story betrifft, hat also die Nummer `2.C`.

✍️ Ein Arbeitspaket sollte etwa 45' für eine Person in Anspruch nehmen. Die totale Anzahl Arbeitspakete sollte etwa Folgendem entsprechen: `Anzahl R-Sitzungen` ╳ `Anzahl Gruppenmitglieder` ╳ `4`. Wenn Sie also zu dritt an einem Projekt arbeiten, für welches zwei R-Sitzungen geplant sind, sollten Sie auf `2` ╳ `3` ╳`4` = `24` Arbeitspakete kommen. Sollten Sie merken, dass Sie hier nicht genügend Arbeitspakte haben, denken Sie sich weitere "Kann"-User Stories für Kapitel 1.2 aus.

## 3 Entscheiden

✍️ Dokumentieren Sie hier Ihre Entscheidungen und Annahmen, die Sie im Bezug auf Ihre User Stories und die Implementierung getroffen haben.

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
