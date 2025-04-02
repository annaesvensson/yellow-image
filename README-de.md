<p align="right"><a href="README-de.md">Deutsch</a> &nbsp; <a href="README.md">English</a> &nbsp; <a href="README-sv.md">Svenska</a></p>

# Image 0.9.3

Bilder in unterschiedlichen Größen hinzufügen.

<p align="center"><img src="SCREENSHOT.png" alt="Bildschirmfoto"></p>

## Wie man eine Erweiterung installiert

[ZIP-Datei herunterladen](https://github.com/annaesvensson/yellow-image/archive/refs/heads/main.zip) und in dein `system/extensions`-Verzeichnis kopieren. [Weitere Informationen zu Erweiterungen](https://github.com/annaesvensson/yellow-update/tree/main/README-de.md).

## Wie man ein Bild hinzufügt

Erstelle eine `[image]`-Abkürzung.

Die folgenden Argumente sind verfügbar, alle bis auf das erste Argument sind optional:
 
`Name` = Dateiname  
`Alt` = Beschreibung des Bildes, mehrere Wörter in Anführungszeichen setzen  
`Style` = Bildstil, z.B. `left`, `center`, `right`  
`Width` = Bildbreite, Pixel oder Prozent  
`Height` = Bildhöhe, Pixel oder Prozent   

Die Bildformate GIF, JPEG, PNG und SVG werden unterstützt. Alle Mediendateien befinden sich im `media`-Verzeichnis. Das `media/images`-Verzeichnis ist zum Speichern von Bildern gedacht. Das `media/thumbnails`-Verzeichnis enthält Miniaturbilder. Man kann auch weitere Verzeichnisse hinzufügen und Dateien so organisieren wie man will.

## Beispiele

Inhaltsdatei mit Bilder in unterschiedlichen Größen:

    ---
    Title: Beispielseite
    ---
    Das ist eine Beispielseite mit Bilder in unterschiedlichen Größen.

    [image photo.jpg Beispiel]

    [image photo.jpg Beispiel - 34%]
    [image photo.jpg Beispiel - 20%]
    [image photo.jpg Beispiel - 10%]

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
`ImageUploadJpegQuality` = JPEG-Qualität für hochgeladene Bilder  
`ImageThumbnailJpegQuality` = JPEG-Qualität für Miniaturbilder  
`ImageJpegExtension` = JPEG-Dateiendung, z.B. `auto`, `.jpeg`, `.jpg`  

## Danksagung

Diese Erweiterung enthält ein Foto von Alejandro Escamilla. Danke für das schöne Foto.

## Entwickler

Anna Svensson. [Hilfe finden](https://datenstrom.se/de/yellow/help/).
