<div class="markdown">

<div>

Unser Ziel als Datenanalysten ist es, die Erkenntnisse aus unseren Daten so aufzubereiten, dass jeder, der sie sieht, ihre Auswirkungen und Handlungsmöglichkeiten klar verstehen kann.

Tableau ist ein Datenanalyse- und Visualisierungstool, das heute in der Industrie weit verbreitet ist. Viele Unternehmen halten es sogar für unverzichtbar für die datenwissenschaftliche Arbeit. Die Benutzerfreundlichkeit von Tableau ergibt sich aus der Tatsache, dass es über eine Drag-and-Drop-Schnittstelle verfügt. Diese Funktion hilft dabei, Aufgaben wie Sortieren, Vergleichen und Analysieren sehr einfach und schnell durchzuführen. Tableau ist außerdem mit mehreren Quellen kompatibel, einschließlich Excel, SQL Server und Cloud-basierten Daten-Repositories, was es zu einer hervorragenden Wahl für Data Scientists macht.

#### In diesem Tutorial werden die folgenden Themen behandelt:

* #### [1\. Einführung in Tableau](#introduction-to-tableau)

    * Überblick
    * Installation
* #### [2\. Getting Started](#getting-started)

    * Tableau-Arbeitsbereich
    * Verbinden mit einer Datenquelle
    * Erstellen einer Ansicht
    * Verfeinern der Ansicht
* #### [3\. Emphasizing the results](#emphasise-the-results)

    * Hinzufügen von Filtern zu der Ansicht
    * Hinzufügen von Farben zur Ansicht
    * Wichtige Ergebnisse
* #### [4\. Kartenansicht](#map-view)

    * Erstellen einer Kartenansicht
    * Ins Detail gehen
    * Identifizieren der Schlüsselpunkte
* #### [5\. Dashboard](#dashboard)

    * Erstellen eines Dashboards
    * Hinzufügen von Interaktivität
* #### [6\. Story](#story)

    * Erstellen einer Story
    * Erstellen einer Schlussfolgerung
* #### [7\. Tableau's integration with R, Python & SQL Server](#tableau_with_R,Python,SQL)

    * Tableau & R
    * Tableau & Python
    * Tableau & SQL Server
* #### [8\. Saving the Work](#saving)

# <a name="introduction-to-tableau"></a>1.Einführung in Tableau

## Überblick.

[Tableau Software](https://www.tableau.com/) ist ein Softwareunternehmen mit Hauptsitz in Seattle, Washington, das interaktive Datenvisualisierungsprodukte mit Schwerpunkt auf Business Intelligence herstellt. Tableau wurde zwischen 1997 und 2002 am Department of Computer Science der Stanford University gegründet[(Wikipedia)](https://en.wikipedia.org/wiki/Tableau_Software)

Die wichtigsten von Tableau angebotenen Produkte sind:

![](assets/1_rdkivl.webp)

### **Tableau Desktop, Tableau Public und Tableau Online**, alle bieten die Erstellung von Datenvisualisierungen und die Auswahl hängt von der Art der Arbeit ab

![](assets/2_sh3myr.webp)

![](assets/3_qe3dfe.webp)

<a name="getting-started"></a>2.Getting Started

In diesem Abschnitt werden wir einige grundlegende Operationen in Tableau erlernen, um uns mit der Oberfläche vertraut zu machen.

## Tableau-Arbeitsbereich

Der Tableau-Arbeitsbereich ist eine Sammlung von Arbeitsblättern, einer Menüleiste, einer Symbolleiste, einer Markierungskarte, Regalen und vielen anderen Elementen, über die wir in den kommenden Abschnitten lernen werden. Sheets können Arbeitsblätter, Dashboards oder Stories sein. Die Abbildung unten zeigt die wichtigsten Komponenten des Arbeitsbereichs. Mehr Vertrautheit werden wir jedoch erlangen, wenn wir mit tatsächlichen Daten arbeiten.

![](assets/4_b8jdpp.webp) Quelle:Tableau.com

## Verbinden mit einer Datenquelle

Um die Arbeit mit Tableau zu beginnen, müssen wir Tableau mit der Datenquelle verbinden. Tableau ist mit einer Vielzahl von Datenquellen kompatibel. Die von Tableau unterstützten Datenquellen erscheinen auf der linken Seite des Eröffnungsbildschirms. Einige häufig verwendete Datenquellen sind Excel, Textdatei, relationale Datenbank oder sogar auf einem Server. Man kann auch eine Verbindung zu einer Cloud-Datenbankquelle wie Google Analytics, Amazon Redshift usw. herstellen.

Der Startbildschirm von Tableau Desktop zeigt die verfügbaren Datenquellen an, mit denen man sich verbinden kann. Es ist auch abhängig von der Version von Tableau, da die kostenpflichtige Version mehr Möglichkeiten bietet. Auf der linken Seite des Bildschirms gibt es einen Bereich "Verbinden", in dem die verfügbaren Quellen hervorgehoben werden. Die Dateitypen werden zuerst aufgelistet, gefolgt von den gängigen Servertypen bzw. den Servern, die kürzlich verbunden wurden. Unter der Registerkarte `Open` können Sie zuvor erstellte Arbeitsmappen öffnen. Tableau Desktop bietet auch einige Beispiel-Arbeitsmappen unter `Sample Workbooks`.

### `Hands On`

![](assets/5_ubfft7.webp)

#### Verbinden mit dem [Sample-Superstore-Datensatz](global-superstore.xlsx)

Wir werden mit einem Beispieldatensatz namens **Superstore-Datensatz** arbeiten, der mit Tableau vorgeladen ist. Wir werden jedoch die Datei von [hier](global-superstore.xlsx) herunterladen, damit wir eine Vorstellung von der Verbindung mit einer Excel-Datenquelle bekommen. Bei den Daten handelt es sich um die eines Superstores. Sie enthält Informationen über Produkte, Verkäufe, Gewinne usw. Unser Ziel als Datenanalysten ist es, die Daten zu analysieren und kritische Bereiche für Verbesserungen in diesem fiktiven Unternehmen zu finden.

### `Schritte`

1.  Importieren der Daten vom Computer in den Tableau-Arbeitsbereich.

2.  Unter der Registerkarte "Sheets" werden drei Blätter sichtbar, nämlich "Orders", "People" und "Returns". Wir werden uns jedoch nur auf die Daten von Orders konzentrieren. Doppelklicken Sie auf das Blatt "Orders", und es öffnet sich wie eine Tabellenkalkulation.

3.  Wir stellen fest, dass die ersten drei Zeilen der Daten etwas anders aussehen und nicht das gewünschte Format haben. Hier verwenden wir den **Dateninterpreter**, der auch unter


### `Hands On`

![](assets/6_f1ydxm.webp)

## Erstellen einer Ansicht

Wir beginnen mit der Erstellung eines einfachen Diagramms. In diesem Abschnitt werden wir unsere Daten kennenlernen und beginnen, Fragen zu den Daten zu stellen, um Erkenntnisse zu gewinnen. Es gibt einige wichtige Begriffe, die uns in diesem Abschnitt begegnen werden.

Dimension".

Messwerte

`Aggregation`

[Dimensionen](https://onlinehelp.tableau.com/current/guides/get-started-tutorial/en-us/get-started-tutorial-drag.html) sind qualitative Daten, wie z. B. ein Name oder ein Datum. Standardmäßig stuft Tableau Daten, die qualitative oder kategoriale Informationen enthalten, automatisch als Dimension ein, z. B. jedes Feld mit Text- oder Datumswerten. Diese Felder erscheinen in der Regel als Spaltenüberschriften für Datenzeilen, z. B. Kundenname oder Bestelldatum, und definieren auch die Granularitätsebene, die in der Ansicht angezeigt wird.

[Measures] (https://onlinehelp.tableau.com/current/guides/get-started-tutorial/en-us/get-started-tutorial-drag.html) sind quantitative numerische Daten. Standardmäßig behandelt Tableau jedes Feld, das diese Art von Daten enthält, als eine Kennzahl, z. B. Verkaufstransaktionen oder Gewinn. Daten, die als Measure klassifiziert sind, können auf Basis einer bestimmten Dimension aggregiert werden, z. B. Gesamtumsatz (Measure) nach Region (Dimension).

Bei der [Aggregation](https://onlinehelp.tableau.com/current/guides/get-started-tutorial/en-us/get-started-tutorial-drag.html) werden die Daten auf Zeilenebene auf eine höhere Kategorie hochgerollt, z. B. die Summe der Verkäufe oder der Gesamtgewinn.

Tableau sortiert die Felder in Measures und Dimensionen automatisch. Bei einer Anomalie kann man sie jedoch auch manuell ändern.

### `Schritte`

1.  Rufen Sie das Arbeitsblatt auf. Klicken Sie auf den Reiter `Blatt 1` unten links im Tableau-Arbeitsbereich.

    ![](assets/7_jgylqq.webp)

2.  Sobald Sie sich im Arbeitsblatt befinden, ziehen Sie aus dem Bereich "Dimensionen" im Datenfenster das Feld "Bestelldatum" auf die Spaltenablage.

    Wenn Sie das "Bestelldatum" auf die Spaltenablage ziehen, wird im Datensatz eine Spalte für jedes Jahr der Bestellungen erstellt. Unter jeder Spalte ist ein 'Abc'-Indikator sichtbar, was bedeutet, dass hier Text oder numerische oder Textdaten gezogen werden können. Wenn wir andererseits `Umsatz` hierher ziehen würden, würde eine Kreuztabelle erstellt werden, die den Gesamtumsatz für jedes Jahr anzeigt.

3.  Ziehen Sie auf der Registerkarte "Messwerte" das Feld "Umsatz" auf die Ablage "Zeilen".

Tableau füllt ein Diagramm mit den als Summe aggregierten Umsätzen auf. Der gesamte aggregierte Umsatz für jedes Jahr nach Bestelldatum wird angezeigt. Tableau füllt immer ein Liniendiagramm für eine Ansicht auf, die ein Zeitfeld enthält, das in diesem Beispiel "Bestelldatum" ist.

### Hands On

![](assets/8_skzimx.webp)

#### _Was vermittelt das obige Liniendiagramm? Nun, es zeigt, dass die Verkäufe recht vielversprechend aussehen und mit der Zeit zu steigen scheinen. Dies ist ein wertvoller Einblick, aber er sagt kaum etwas über die Produkte aus, die zur Umsatzsteigerung beitragen. Lassen Sie uns weiter eintauchen, um mehr Erkenntnisse zu erhalten.

## Verfeinerung der Ansicht

Lassen Sie uns tiefer eintauchen und versuchen, weitere Erkenntnisse darüber zu gewinnen, welche Produkte zu mehr Umsatz führen. Beginnen wir damit, die Produktkategorien hinzuzufügen, um die Umsatzsummen auf eine andere Art und Weise zu betrachten.

### `Schritte`

1.  Kategorie" befindet sich unter dem Bereich "Abmessungen". Ziehen Sie sie in die Spaltenablage und platzieren Sie sie neben "JAHR(Bestelldatum)". Die `Kategorie` sollte rechts von `Jahr` platziert werden. Dadurch ändert sich die Ansicht sofort von einer Linie zu einem Balkendiagramm. Das Diagramm zeigt die gesamten `Umsätze` für jedes `Produkt` nach Jahr an.

    Mehr erfahren

    Um Informationen zu jedem Datenpunkt (d. h. jeder Markierung) in der Ansicht anzuzeigen, bewegen Sie den Mauszeiger über einen der Balken, um eine QuickInfo einzublenden. Der Tooltip zeigt den Gesamtumsatz für diese Kategorie an. Hier ist die QuickInfo für die Kategorie "Bürobedarf" für 2016:

    ![](assets/9_n0mjak.webp)

    Um der Ansicht Beschriftungen hinzuzufügen, klicken Sie in der Symbolleiste auf "Beschriftungen einblenden".

    ![](assets/10_h6tfyy.webp)

    Das Balkendiagramm kann auch horizontal statt vertikal angezeigt werden. Klicken Sie dazu auf "Swap" in der Symbolleiste.  

    ![](assets/tableau_11.webp)

 2\. Die obige Ansicht zeigt sehr schön die Umsätze nach Kategorien, d.h. Möbel, Bürobedarf und Technik. Wir können auch ableiten, dass der Umsatz mit Möbeln schneller wächst als der Umsatz mit Büroartikeln, außer 2016. Daher ist es ratsam, die Verkaufsanstrengungen auf Möbel statt auf Büroartikel zu konzentrieren. Aber Möbel sind eine große Kategorie und bestehen aus vielen verschiedenen Artikeln. Wie können wir erkennen, welcher Möbelartikel zum maximalen Umsatz beiträgt?

Um uns bei der Beantwortung dieser Frage zu helfen, entscheiden wir uns, die Produkte nach "Unterkategorie" zu betrachten, um zu sehen, welche Artikel die großen Verkaufsschlager sind. Nehmen wir an, dass wir für die Kategorie **Möbel** nur Details über Bücherregale, Stühle, Einrichtungsgegenstände und Tische betrachten wollen. Wir doppelklicken oder ziehen die Dimension "Unterkategorie" in die Ablage "Spalten".

