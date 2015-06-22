AngularJS
=========

###Einleitung
AngularJS habe ich mithilfe von folgenden Quellen erarbeitet und studiert:
* [AngularJS.de](https://angularjs.de/buch)
* [Codecademy.com](http://www.codecademy.com/)

###Inhalsverzeinis
* [Was ist AngularJS](#FirstParagraph)
* [Vorteile von AngularJS](#SecondParagraph)
* [Databinding](#ThirdParagraph)
* [AngularJS Komponenten](#FourthParagraph)

<a name="FirstParagraph"></a>
###Was ist AngularJS?
AngularJS ist in wenigen Strichpunkten zusammengefasst:
* Ein JavaScript-Framework für dynamische Webapplikationen
* Für die Entwicklung von Single-Page-Apps gedacht
* Entwicklung von Google und dort Produktiveinsatz
* Ein Open-Source-Projekt
* Auf gute Testbarkeit ausgelegt

<a name="SecondParagraph"></a>
###Vorteile von AngularJS
**Code-Reduktion**

AnuglarJS macht einen Grossteil des Codes,. den man normalerweise schreibt, überflüssig. Der Quellcode ist viel kleiner als z.B. bei jQuery.

**Testbarkeit und Restrukturierung**

AngularJS benutzt Dependecy Injection durch und durch. Dependecy Injection sorgt für eine sehr gute Testbarkeit, Code-Redution und Restrukturierung.

**Wiederverwendbare Komponenten und Lesbarkeit**

AngularJS kann das HTML-Vokabular über Direktiven erweitern. Die Verwendung von Direktiven bringt folgende Vorteile:
* Die Lesbarkeit wird deutlich gesteigert durch logische Bennenung und Weglassen von Elementen.
* Automatisches Entstehen von Komponenten, die sich sehr gut testen und wiederverwnden lassen. (DOM-Testen ist einfach mit AngularJS)

**Verwendung der Datentypen von JavaScript**

Der Einstieg geht in AngularJS sehr schnell, da die normalen Datentypen von JavaScript verwendet werden. Dadurch lassen sich fremde Bibliotheken einfach einbinden.

<a name="ThirdParagraph"></a>
###Databinding - einfach und bidirektional
In der einfachen JavaScript-Programmierung werden Änderungen direkt im DOM vom Event-Handler ausgeführt.([Mehr zu JavaScript](https://github.com/michaelhaenzi/javascript))
Bei bidirektionalem ändert man nur das Model. Änderungen vom Model werden vom Framework in den DOM übertragen:
* Sorgt für klare Trennung
* Sorgt für verständlichem Code

  *In der Betriebsart bidirektional können bei der Datenübertragung Signale in beiden Richtungen fließen. Zwischen Sender und Empfänger gibt es zwei Kanäle: einen Hin- und einen Rückkanal. Jeder Teilnehmer einer bidirektionalen Verbindung kann somit Sender oder Empfänger sein.*
  [Quelle](http://www.itwissen.info/definition/lexikon/Bidirektional-bidirectional.html)

![Databinding](https://github.com/michaelhaenzi/angularjs/blob/master/databinding.PNG)

**Einfaches Databinding (One-Way)**

Einfache Databinding wird den meisten Entwicklern vertraut sein. Es gibt ein Model, welches die Daten bereitstellt und ein Template, welches das Aussehen liefert. Diese werden verschmolzen und als View an den Benutzer geschickt.

Änderung am Model und im View (z.B. eine Eingabe im Inputfeld) werden nicht automatisch aktualisiert. Der Entwickler muss deshalb sich selber um die Synchronisation von View und Model kümmern.

**Bidirektionales Databinding (Two-Way)**

Beim bidirektionalen wird eine Verknüpfung zwischen Elementen im View und Datenstrukturen im Model hergestellt.
Der Vorteil dürfte offensichtlich sein. Die manuelle Synchronisation fällt weg und damit auch eine Menge Arbeit und fehleranfälliger Code.

<a name="FourthParagraph"></a>
###Überblick der wichtigsten Komponenten

![Komponenten](https://github.com/michaelhaenzi/angularjs/blob/master/components.PNG)
