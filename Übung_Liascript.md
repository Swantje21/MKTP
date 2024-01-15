# Übung

## Einrichtung

Sie benötigen einen Laptop/Tablet und den Liveeditor von Liascript:

https://liascript.github.io oder einfach LiaScript im Browser suchen

<iframe src="https://liascript.github.io" style="border:0px;width:100%;height:500px" allowfullscreen="true" webkitallowfullscreen="true" mozallowfullscreen="true"></iframe>

## Textstrukturierung

Überschriften werden durch eine einfache Raute erzeugt. Die Anzahl der Rauten bestimmt die Ordnung der Überschriften. Es muss ein Leerzeichen zwischen den Rauten und dem Überschriftentext sein.

Einfache Textblöcke werden unformatiert eingegeben. Sie müssen jedoch mit einer Leerzeile von anderen Blöcken getrennt sein.
Ohne Leerzeile wird ein Satz zum Block hinzugerechnet.

> Spitzklammern erzeugen einen farblich markierten Bereich, der der Hervorhebung von 
> Textblöcken dienen kann.

> "Fügt man einen abgesetzten und durch zwei Bindestriche markierten Urheber des Zitates und eine Leerzeile hinzu, wird der Textblock als Zitat hervorgehoben."
>
> -- Liascript Jünger 

Unterüberschriften innerhalb des Blocks
----

Große Unterüberschrift innerhalb des Blocks
====

----

Für eine durchgezogene Linie muss vor und nach den Bindestrichen ein Leerzeile bleiben.


## Textformatierung

_kursiv_ auch *kursiv*

__fett__ auch **fett**

___kursiv___ und ***fett***

~durchgestrichen~

~~unterstrichen~~

Text normal ^hochgestellter Text^

`unformatierter Code` zum Beispiel für Inline-Code `<title>Titel</title>`

## Multimedia

### Bilder

{{1-2}}
***************************

Verweis auf Externe Bilder:

``` html
![alt](https://...)
![alt](https://... "titel")
```

Beispiel:
![Annunciation of the brith of Christ](https://upload.wikimedia.org/wikipedia/commons/5/51/Leonardo_da_Vinci_Annunciation.jpg)



***********************

{{2}}
************************

Projektinterne Bilder:

``` html
![alt](/pic/image.jpg)
![alt](/pic/image.jpg "titel")
```

**********************

### Audio

* Syntax: `?[ein Pferd](https://www.w3schools.com/html/horse.mp3 "höre ein Pferd wiehern")`
* Example:

  ?[ein Pferd](https://www.w3schools.com/html/horse.mp3 "höre ein Pferd wiehern")

### Video

**Movie-notation: `!?[alt-text](movie-url)`**

- YouTube: `!?[The Future of Programming](https://www.youtube.com/watch?v=8pTEmbeENF4)`

  !?[The Future of Programming](https://www.youtube.com/watch?v=8pTEmbeENF4)

- relative path: `!?[Something about math](vid/math.mp4)`

  !?[Something about math](vid/math.mp4)

- > # List of supported Video Platforms
  >
  > * [DailyMotion](https://www.dailymotion.com)
  > * [PeerTube](https://peertube.tv)
  > * [TeacherTube](https://TeacherTube.com)
  > * [Video TU-Freiberg](https://video.tu-freiberg.de)
  > * [Vimeo](https://Vimeo.com)
  > * [YouTube](https://YouTube.com)

### Code

``` js
let text = 'Hello, World';
text;
```
<script>
    @input
</script>

### Und mehr

[SketchFab](https://sketchfab.com): `??[Die Stadt Düren 1634](https://sketchfab.com/3d-models/dueren1634-citymodel-c-f1f1c5c63a484303b953621343c75075)`

  ??[Dueren 1634](https://sketchfab.com/3d-models/dueren1634-citymodel-c-f1f1c5c63a484303b953621343c75075)

## Animationen

    {{0}}
Wie in Powerpoint können Textblöcke der Reihe nach erscheinen. 

    {{1-3}}
Dieser Block kommt nach dem ersten Klick. Dies markiert man mit zwei geschweiften Klammern `{{in(-out)}}`, die in der Mitte durch Zahlen angeben, wann der Block erscheint und (optional) wann er wieder verschwindet.

    {{2-3}}
Dieser Block erscheint ab Schritt 2 und verschwindet bei 3, markiert durch `{{2-3}}`

    {{3}}
Um einen Block ab einem Schritt stehen zu lassen gibt man nur den entsprechenden Schritt als einzelne Zahl an. Dieser hier erscheint bei 3 und bleibt auch bei 4.

    {{3-4}}
Dieser Block kommt bei drei und geht bei 4, markiert durch `{{3-4}}`

    {{4}}
Dieser Block erscheint bei 4.

## Quizze

### Textquiz

Wie heißt die hier vorangestellte Sprache?

[[LiaScript]]

### Single Choice

Anzahl und Ordnung der Optionen ist beliebig.

[( )] Diese Wahl ist falsch.
[(X)] <-- __Richtig__
[( )] Auch falsch.

### Multiple Choice

Alle markierten Zeilen müssen ausgewählt werden:

[[ ]] nicht ausgewählt
[[X]] <-- __Richtig__
[[ ]] auch falsch.
[[X]] __auch Richtig__

### Matrix

Kombination von Single- und Multiple-Choice Quizzen:

[[Head 1] [_Head 2_] [**Head 3**]]
[  [X]        [ ]         [X]    ]  Weitere
[  ( )        (X)         ( )    ]  Zeilen...

### Hilfen

Hilfen können mit `[[?]]` an alle Quizze angehängt werden:

[[LiaScript]]
[[?]] Tipp 1
[[?]] Tipp 2
[[?]] ...




