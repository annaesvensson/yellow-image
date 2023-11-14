<p align="right"><a href="README-de.md">Deutsch</a> &nbsp; <a href="README.md">English</a> &nbsp; <a href="README-sv.md">Svenska</a></p>

# Image 0.8.19

Lägg till bilder och miniatyrbilder.

<p align="center"><img src="image-screenshot.png?raw=true" alt="Skärmdump"></p>

## Hur man installerar ett tillägg

[Ladda ner ZIP-filen](https://github.com/annaesvensson/yellow-image/archive/refs/heads/main.zip) och kopiera den till din `system/extensions` mapp. [Läs mer om tillägg](https://github.com/annaesvensson/yellow-update/tree/main/README-sv.md).

## Hur man lägger till en bild

Skapa en `[image]` förkortning.

Följande argument är tillgängliga, alla utom det första argumentet är valfria:
 
`Name` = filnamn  
`Alt` = beskrivning av bilden, placera flera ord i citattecken  
`Style` = bildstil, t.ex. `left`, `center`, `right`  
`Width` = bildbredd, pixel eller procent  
`Height` = bildhöjd, pixel eller procent  

Bildformaten GIF, JPG, PNG och SVG stöds. Alla mediefiler finns i `media` mappen.
Mappen `media/images` är platsen för att lagra dina bilder. Mappen `media/thumbnails` innehåller miniatyrbilder. Du kan också skapa ytterligare mappar och organisera filer som du vill.

## Exempel

Lägga till en bild, olika beskrivningar:

    [image photo.jpg Exempel]
    [image photo.jpg "Detta är en exempelbild"]
    [image photo.jpg "Detta är en särskilt lång beskrivning"]

Lägga till en bild, olika stilar:

    [image photo.jpg Exempel left]
    [image photo.jpg Exempel center]
    [image photo.jpg Exempel right]

Lägga till en bild, olika storlekar:

    [image photo.jpg Exempel right 50%]
    [image photo.jpg Exempel right 64 64]
    [image photo.jpg Exempel right 320 200]

Lägga till en bild, olika storlekar med standardstilen:

    [image photo.jpg Exempel - 50%]
    [image photo.jpg Exempel - 64 64]
    [image photo.jpg Exempel - 320 200]

## Inställningar

Följande inställningar kan konfigureras i filen `system/extensions/yellow-system.ini`:

`ImageUploadWidthMax` = maximal bredd för uppladdning, större bilder minskas i storlek  
`ImageUploadHeightMax` = maximal höjd för uppladdning, större bilder minskas i storlek  
`ImageUploadJpgQuality` = JPG-kvalitet för uppladdade bilder  
`ImageThumbnailJpgQuality` = JPG-kvalitet för miniatyrbilder  

## Tack

Detta tillägg innehåller ett [foto](https://unsplash.com/photos/xII7efH1G6o) av Alejandro Escamilla. Tack för det vackra fotot.

## Utvecklare

Anna Svensson. [Få hjälp](https://datenstrom.se/sv/yellow/help/).
