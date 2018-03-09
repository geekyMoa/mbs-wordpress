---
title: Installera WP
date: 2018-03-08 14:06:07
---

## Ladda ner

Gå till http://wordpress.org och klicka på "Ladda ner". Du kommer få ner en `.zip`-fil. Packa upp den genom att dubbelklicka på den och titta på innehållet. Notera att det finns en `wp-content`-mapp och en fil som heter `wp-config-sample.php`. Vi kommer återkomma till dessa två.

## Flytta till rätt mapp på din dator

Öppna utforskaren i Windows. Navigera till `C:/MAMP/htdocs`. I denna mapp ska du lägga hela wordpress-mappen som du just laddade ner, inklusive alla filer i den mappen. Det enklaste är att dra och släppa `wordpress`-mappen i `htdocs`-mappen.

Dina WordPress-filer ska nu ha sökvägen `C:/MAMP/htdocs/wordpress`.

## phpMyAdmin

phpMyAdmin är ett program för att administrera databaser, och vi ska använda det för att skapa databasen till vår WordPress-sajt.

Öppna programmet MAMP. Om du inte hittar det på skrivbordet, använd sökfunktionen i Windows (förstoringsglaset i närheten av Start-menyn). MAMP har ett val som heter ungefär "Open WebStart page" (exakta formuleringen kan skilja sig lite åt beroende på version av MAMP). Klicka på det valet.

Du bör mötas av en sida som ser ut så här:

![alt text](/images/mamp-webstart.png "MAMP Webstart")

Under rubriken "MySQL" finns en liten länk med texten "phpMyAdmin", klicka på den.

![alt text](/images/phpmyadmin.png "phpMyAdmin")

Klicka på fliken "Databases" och hitta fältet "Create database". Välj ett namn utan svenska tecken och kom ihåg vad du döpte din nya databas till - du behöver namnet senare. Clicka på knappen "Create".

## Berätta för WordPress om databasen

Nu ska du kunna gå till din lokala WordPress-installation och berätta för WordPress om din databas! Gå till http://localhost/wordpress. Läs igenom texten och klicka på knappen "Då kör vi!" längst ned.

Här behöver du namnet på din databas som du skapade, det fyller du i i fältet "Databasnamn". Användarnamn och lösenord är `root`och `root` (samma användarnamn som lösenord). Dessa uppgifter finns på MAMP:s webstart-sida.

## Installera WordPress!

Följ instruktionerna på skärmen! Tänk på att den sajt du nu skapar inte kommer finnas tillgänglig för andra på internet, utan _bara_ kommer synas för dig som använder just den här datorn, så du behöver inte hitta på något krångligt lösenord. Om du däremot gör detta själv med en riktig webbplats så är det väldigt viktigt att välja ett långt och starkt lösenord!
