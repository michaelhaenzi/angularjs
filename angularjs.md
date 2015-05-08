AngularJS
=========

###Einleitung

Ich habe AngularJS mit der Webseite [Codecademy](www.codecademy.com) gelernt. *"Codecademy versteht sich als einfache, kurzweilige und interaktive Möglichkeit, Programmieren zu lernen. Die Website ist seit kurzem live und ist im Kern ein interaktives Programmier-Tutorial."*


###Was ist AngularJS?

Angular JS ist ein JavaScript Clientseitiges basiertes Framework. Es wird von Google entwickelt und gratis zur verfügung gestellt. Angular JS ist geeignet für Single-Page-Applikationen. Das bedeutet, dass die meisten Daten beim aufrufen der Webseite geladen werden. Bei einer Änderung des Linkes (URL) wird nicht die ganze Seite aktualisiert, sondern nur die benötigten Daten werden per Ajax nachgeladen.

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

![Generallisierung Bild](generallisiert.png)
*Bild von Codecademy*

1. User besucht die AngularJS Applikation.
2. Die HTML-Seite(auch View genannt) gibt die Applikationes Daten an. Also Direktiven, Expressions, Filter usw. Die Direktiven binden sich nun an die HTML Elemente.
3. Wenn der Benutzer ein Element anklickt, welches eine Direktive beinhaltet, dann wird die AngularJS Funktion ausgeführt.
4. Die Funktion im Kontroller aktualisiert die Daten.
5. Die HTML-Seite verändert sich automatisch ohne die Seite neu zuladen.

Durch das dass man die Daten per Aufruf verankert und dann aktualisiert, muss man die Seite nicht neu laden.





###Module

###Scopes & Controller
