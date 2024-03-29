# Lern-Bericht
Lilac: Lorenzo Lai, Justus Meister, Angel Angelov, Julian Hitz, Enrique Schneider

## Einleitung

In unserem Projekt haben wir ein unterhaltsames Jump-and-Run-Spiel entwickelt, das dem bekannten "Dino Run" von Google Chrome ähnelt, aber zusätzliche Features enthält, um das Spielerlebnis noch spannender und herausfordernder zu gestalten.

## Was haben wir gelernt?

Wir haben in diesem Projekt gelernt, wie man Objekte in Unity in einer Schleife selbst bewegen kann.

## Beschreibung

Um Gegenstände zu bewegen, haben wir den folgenden Code eingesetzt. Als erstes definierten wir eine Klasse namens "BoxMovement", welche von der MonoBehaviour-Klasse erbt. Die Klasse enthält eine öffentliche Variable "speed", die auf 10 initialisiert wird. Eine Variable "run" vom Typ boolean und eine weitere Variable "rb" vom Typ "Rigidbody2D" werden ebenfalls definiert. In der Start()-Methode wird die "Rigidbody2D"-Komponente des Gameobjects geholt und der Variable "rb" zugewiesen. Die Variable "run" wird auf "true" gesetzt. Die Update()-Methode wird einmal pro Frame aufgerufen. Wenn die Variable "run" auf "true" gesetzt ist, wird die Geschwindigkeit der "Rigidbody2D"-Komponente auf einen neuen Vector2 gesetzt, wobei der X-Wert gleich 0 minus der Variablen "speed" ist und der Y-Wert gleich 0 ist. Dann wird geprüft, ob die X-Position des Gameobjects kleiner als -12 ist. Wenn dies der Fall ist, wird die Position des Gameobjects auf einen neuen Vector2 mit einem X-Wert von 14 und einem Y-Wert von -2 gesetzt. Zusammengefasst bewirkt dieser Code, dass ein Gameobject mit einer "Rigidbody2D"-Komponente in eine bestimmte Richtung bewegt wird, bis es einen bestimmten Punkt erreicht. An diesem Punkt wird das Gameobject zurückgesetzt und die Bewegung beginnt von vorne.



```csharp
public int speed = 10;

bool run;

private Rigidbody2D rb;

// Start is called before the first frame update
public void Start()
{
    rb = GetComponent<Rigidbody2D>();
    run = true;
}

// Update is called once per frame
public void Update()
{
    if(run == true)
    {
        rb.velocity = new Vector2(0 - speed, 0);

        if(transform.position.x < -12)
        {
            transform.position = new Vector2(14, -2);
        }
    }
}
```


![MagigRun](https://user-images.githubusercontent.com/110893098/229737825-134413c3-82f3-4bde-b4ee-f0aa6d8caf85.gif)


## Verifikation

Quelle 1: Dieser Text beschreibt den Code, der verwendet wurde, um ein Gameobject in Unity mit einer Rigidbody2D-Komponente in eine bestimmte Richtung zu bewegen, bis es einen bestimmten Punkt erreicht, an dem es zurückgesetzt wird und die Bewegung von vorne beginnt.

Quelle 2: Dieser Code sagt einem Objekt, wie schnell es sich bewegen soll "speed". Wenn "run" läuft, bewegt es sich in eine Richtung. Wenn das Objekt an einem bestimmten Punkt angelangt ist, wird es wieder zurückgesetzt und die Bewegung beginnt von vorne.

Quelle 3: Dieses GIF zeigt, wie der Spieler über das bewegende Objekt springen kann.

# Reflektion zum Arbeitsprozess

**Was lief gut** :
Wir haben regelmässig Besprechungen abgehalten, um sicherzustellen, dass alle auf dem gleichen Stand sind und den Fortschritt der Arbeit verfolgen konnten. Wenn ein Mitglied des Teams abwesend war, haben wir uns zusätzlich abgestimmt, um sicherzustellen, dass die Arbeit nahtlos weitergehen konnte.


**Was lief nicht gut** :
Während des Projekts gab es eine Herausforderung, als ein Mitglied des Teams nicht verfügbar war. Wir haben jedoch schnell gehandelt, um unsere Arbeitsweise anzupassen und sicherzustellen, dass wir unsere Ziele dennoch erreichen konnten.


**VBV** : Für das nächste Mal haben wir beschlossen, den Code, den wir jede Woche geschrieben haben, in unseren Gruppenchat zu stellen. Dadurch haben alle Gruppenmitglieder Zugriff auf den Code und können selbstständig arbeiten, ohne von einem bestimmten Teammitglied abhängig zu sein. Das sollte uns helfen, flexibler zu arbeiten und eventuellen Ausfällen besser zu begegnen.
