AngularJS
=========

###Einleitung
AngularJS habe ich mithilfe von folgenden Quellen erarbeitet und studiert:
* [AngularJS.de](https://angularjs.de/buch)
* [Codecademy.com](http://www.codecademy.com/)

###Was ist AngularJS?
AngularJS ist in wenigen Strichpunkten zusammengefasst:
* Ein JavaScript-Framework für dynamische Webapplikationen
* Für die Entwicklung von Single-Page-Apps gedacht
* Entwicklung von Google und dort Produktiveinsatz
* Ein Open-Source-Projekt
* Auf gute Testbarkeit ausgelegt
* Test

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


###Der Anfang von einer AngularJS Applikation

```html
<html ng-app>
<head>
  <meta charset="utf8" />
  <title>AngularJS Tutorial</title>
  <link rel="stylesheet" href="//netdna.bootstrapcdn.com/bootstrap/3.0.3/css/bootstrap.min.css">
</head>
<body>
  <!-- Lokale Angular Datei (https://angularjs.org/) -->
  <script src="js/angular.js"></script>
</body>
</html>
```
Durch das Attribut `ng-app` im *html*-Tag erkennt AngularJS unsere Seite nun als AngularJS-Applikation. AngularJS durchsucht dadurch die Seite nach speziellen Tags und Attributen, die zum Framework gehören. Diese heißen in AngularJS Direktiven.

###Direktiven

AngularJS hat spezielle Tags wie `ng-app`, die wir Direktiven nennen. Diese erweitern den Sprachumfang von HTML. Direktiven von AngularJS erkennst du an dem Präfix `ng-.` Die Direktiven helfen dir, große Teile eine Applikation ohne eine Zeile Code zu schreiben.

###Expressions

Expressions sind viel mächtiger, als sie im ersten Moment erscheinen. Expressions erlauben uns, Daten zu manipulieren und zu kombinieren.

###Filter

Filter sind Formate oder Definitionen, welche man angeben kann, um z.B. Währung, Datum oder Uhrzeit automatisch anzupassen.


###Beispiel

```html
<!-- ng-show Direktive -->
<input type="text" ng-model="today">
<!-- im {{today.date}} wird der aktuelle Wert in der Html-Seite aufgezeig, dies ist eine Expression-->
<!-- | date ist ein Filter und passt das Datum ins definierte Format an -->
<p>Du suchst gerade nach: {{today.date}} | date</p>
```
###Die Verallgemeinerung

![Generallisierung Bild](https://github.com/michaelhaenzi/angularjs/blob/master/generallisiert.PNG)
*Bild von Codecademy*

1. User besucht die AngularJS Applikation.
2. Die HTML-Seite(auch View genannt) gibt die Applikationes Daten an. Also Direktiven, Expressions, Filter usw. Die Direktiven binden sich nun an die HTML Elemente.
3. Wenn der Benutzer ein Element anklickt, welches eine Direktive beinhaltet, dann wird die AngularJS Funktion ausgeführt.
4. Die Funktion im Kontroller aktualisiert die Daten.
5. Die HTML-Seite verändert sich automatisch ohne die Seite neu zuladen.

Durch das dass man die Daten per Aufruf verankert und dann aktualisiert, muss man die Seite nicht neu laden.





###Module

###Scopes & Controller
