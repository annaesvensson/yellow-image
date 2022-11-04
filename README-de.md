<p align="right"><a href="README-de.md">Deutsch</a> &nbsp; <a href="README.md">English</a> &nbsp; <a href="README-sv.md">Svenska</a></p>

# Image 0.8.18

Bilder in unterschiedlichen Größen.

<p align="center"><img src="image-screenshot.png?raw=true" alt="Bildschirmfoto"></p>

## Wie man ein Bild hinzufügt

Erstelle eine `[image]`-Abkürzung.

Die folgenden Argumente sind verfügbar, alle bis auf das erste Argument sind optional:
 
`Name` = Dateiname  
`Alt` = Beschreibung des Bildes, mehrere Wörter in Anführungszeichen setzen  
`Style` = Bildstil, z.B. `left`, `center`, `right`  
`Width` = Bildbreite, Pixel oder Prozent  
`Height` = Bildhöhe, Pixel oder Prozent   

Die Bildformate GIF, JPG, PNG und SVG werden unterstützt. Alle Mediendateien befinden sich im `media`-Verzeichnis. Das `media/images`-Verzeichnis ist zum Speichern von Bildern gedacht. Das `media/thumbnails`-Verzeichnis enthält Miniaturbilder. Man kann auch weitere Verzeichnisse hinzufügen und Dateien so organisieren wie man will.

## Beispiele

Bild hinzufügen, unterschiedliche Beschreibungen:

    [image photo.jpg Beispiel]
    [image photo.jpg "Dies ist ein Beispielbild"]
    [image photo.jpg "Dies ist eine besonders lange Beschreibung"]

Bild hinzufügen, unterschiedliche Stile:

    [image photo.jpg Beispiel left]
    [image photo.jpg Beispiel center]
    [image photo.jpg Beispiel right]

Bild hinzufügen, unterschiedliche Größen:

    [image photo.jpg Beispiel right 50%]
    [image photo.jpg Beispiel right 64 64]
    [image photo.jpg Beispiel right 320 200]

Bild hinzufügen, unterschiedliche Größen mit dem Standardstil:

    [image photo.jpg Beispiel - 50%]
    [image photo.jpg Beispiel - 64 64]
    [image photo.jpg Beispiel - 320 200]

## Einstellungen

Die folgenden Einstellungen können in der Datei `system/extensions/yellow-system.ini` vorgenommen werden:

`ImageUploadWidthMax` = maximale Breite zum Hochladen, größere Bilder werden verkleinert  
`ImageUploadHeightMax` = maximale Höhe zum Hochladen, größere Bilder werden verkleinert  
`ImageUploadJpgQuality` = JPG-Qualität für hochgeladene Bilder  
`ImageThumbnailJpgQuality` = JPG-Qualität für Miniaturbilder  

## Installation

[Erweiterung herunterladen](https://github.com/annaesvensson/yellow-image/archive/main.zip) und die ZIP-Datei in dein `system/extensions`-Verzeichnis kopieren. [Weitere Informationen zu Erweiterungen](https://github.com/annaesvensson/yellow-update/tree/main/README-de.md).

Diese Erweiterung enthält ein [Bild](https://unsplash.com/photos/xII7efH1G6o) von Alejandro Escamilla.

## Entwickler

Anna Svensson. [Hilfe finden](https://datenstrom.se/de/yellow/help/).
