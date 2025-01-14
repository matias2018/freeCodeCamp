---
id: 587d7fb3367417b2b2512bfb
title: 'Wie man package.json, den Kern eines jeden Node.js-Projekts oder npm-Pakets, verwendet'
challengeType: 2
forumTopicId: 301528
dashedName: how-to-use-package-json-the-core-of-any-node-js-project-or-npm-package
---

# --description--

Bei der Bearbeitung dieser Aufgaben musst du deinen Code nach einer der folgenden Methoden schreiben:

- Klone <a href="https://github.com/freeCodeCamp/boilerplate-npm/" target="_blank" rel="noopener noreferrer nofollow">diese GitHub-Repo</a> und schließe dein Projekt lokal ab.
- Benutze <a href="https://replit.com/github/freeCodeCamp/boilerplate-npm" target="_blank" rel="noopener noreferrer nofollow">unser Replit-Starterprojekt</a>, um diese Aufgabe fertigzustellen.
- Verwende einen Site-Builder deiner Wahl, um das Projekt fertigzustellen. Achte darauf, alle Dateien aus unserer GitHub-Repo zu integrieren.

Wenn du Replit verwendest, folge diesen Schritten, um das Projekt einzurichten:

-   Beginne, indem du das Projekt in Replit importierst.
-   Als nächstes wird ein `.replit`-Fenster angezeigt.
-   Wähle `Use run command` aus und klicke die `Done`-Schaltfläche.

Wenn du fertig bist, stelle sicher, dass eine funktionierende Demo deines Projekts irgendwo öffentlich gehostet wird. Then submit the URL to it in the Solution Link field.

Die `package.json`-Datei stellt das Zentrum eines Node.js-Projekts oder npm-Pakets dar. Es speichert Informationen über dein Projekt, ähnlich wie der &lt;head>-Abschnitt eines HTML-Dokuments den Inhalt einer Webseite beschreibt. Es besteht aus einem einzigen JSON-Objekt, in dem Informationen in Schlüssel-Wert-Paaren gespeichert sind. Es gibt dort nur zwei Pflichtfelder: "name" und "version". Es ist jedoch empfehlenswert, zusätzliche Informationen über dein Projekt anzugeben, die für zukünfige Benutzer oder Maintainer nützlich sein könnten.

Wenn du dir den Dateibaum deines Projekts ansiehst, wirst du die package.json-Datei auf der obersten Ebene des Baums finden. Das ist die Datei, die du in den nächsten paar Aufgaben verbessern wirst.

Eine der häufigsten Angaben in dieser Datei stellt das `author`-Feld dar. Es gibt an, wer das Projekt erstellt hat, und kann aus einer Zeichenfolge oder einem Objekt mit Kontaktdaten oder anderen Informationen bestehen. Für größere Projekte wird ein Objekt empfohlen, aber eine einfache Zeichenfolge wie das folgende Beispiel ist für dieses Projekt ausreichend.

```json
"author": "Jane Doe",
```

# --instructions--

Trage in der package.json-Datei deinen Namen als `author` des Projekts ein.

**Hinweis:** Denk daran, dass du JSON schreibst, daher müssen alle Feldnamen in doppelten Anführungszeichen (") gesetzt und durch ein Komma (,) getrennt werden.

# --hints--

package.json sollte über einen gültigen "author"-Schlüssel verfügen

```js
(getUserInput) =>
  $.get(getUserInput('url') + '/_api/package.json').then(
    (data) => {
      var packJson = JSON.parse(data);
      assert(packJson.author, '"author" is missing');
    },
    (xhr) => {
      throw new Error(xhr.responseText);
    }
  );
```

# --solutions--

```js
/**
  Backend challenges don't need solutions, 
  because they would need to be tested against a full working project. 
  Please check our contributing guidelines to learn more.
*/
```
