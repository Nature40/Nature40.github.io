---
subheadline: Natur 4.0 | Sensing Biodiversity
title:  "Projektbereich Sensornetzwerk"
teaser: "Um die notwendige Datendichte in NatNet zu erreichen, ist eine kontinuierliche, mobile und den Mikrohabitatskalen von Pflanzen und Tieren Rechnung tragende Datenerfassung nach dem Prinzip des Crowdsensing notwendig. Im Projektbereich Sensornetznetzwerk (SN) werden die hierfür verwendeten Sensorboxen realisiert und zusammen mit der Koordination im Natur 4.0 Lab deren Einrichtung, Wartung und Betreuung organisiert."
slug: sensornetzwerk
---

<div class="row">
<div class="medium-4 medium-push-8 columns" markdown="1">
<div class="panel radius" markdown="1">
**Inhaltsübersicht**
{: #toc }
*  TOC
{:toc}
</div>
{% include next-previous-page-in-category content='about' %}
</div><!-- /.medium-4.columns -->

<div class="medium-8 medium-pull-4 columns" markdown="1">


## Aufgaben
Im Kern des Projektbereichs SN steht die Datenerfassung mittels Kombinationen von kommunizierenden Umweltsensorboxen und Plattformen. Hierfür werden modulare Sensorboxen entwickelt (Roverbox, Baumbox, Rehbox, Bürgerbox etc.), die GPS (Standort, Bewegungsprofil), Gyrometer (Mikrobewegungsmuster, Standort als GPS-Alternative), meteorologische Sensorik (Mikroklima), Lichtintensität (indirekte Strukturinformation im Bestand), Mikrophon (akustische Fernerkundung der Biodiversität), optische Fernerkundungs- (Artenerkennung, Phänologie, Physiologie, Morphologie etc.) und Radarsensoren (Insektenerfassung), Saftflussmessungen, Dendrometer (Phänologie, Stress) u.a. integrieren können. Viele der bildhaften Datensätze unterscheiden sich dabei von herkömmlich verwendeten Fernerkundungsinformationen, da sie in unmittelbarer Nähe zum jeweils beobachteten Objekt und an dessen Standort, also unterhalb einer ggf. behindernden Wolken- oder Kronenschicht aufgenommen werden. Die Kommunikation und Datenweitergabe zur zentralen NatDB erfolgt über autarke Peer-to-Peer- bzw. Device-to-Device-Netzwerke. In enger Abstimmung mit dem Projektbereich Umweltmodellierung wird auch die möglichst effektive Datenaufnahme und Datenweitergabe realisieren. Dies umfasst auch die passgenau auf die in NatNet implementierten Modelle abgestimmte Vorverarbeitung und Selektion von Datenströmen zur Reduzierung der zu kommunizierenden Datenmenge. 

## Beitrag zu Natur 4.0
Der Projektbereich SN legt mit der zentralen Datenerfassungskomponente die Grundlagen für NatNet. Die über die Zeit erreichte, detaillierte Erfassung von Umweltvariablen realisiert gemeinsam mit den Aktivitäten im Projektbereich Umweltmodellierung einen bisher nicht erreichten Detailgrad im Landschaftsmonitoring. Damit wird die naturschutzfachliche Beobachtung auf eine neue Basis gestellt und ein Forschungswerkzeug zur Auflösung des Kompromisses zwischen Detailgrad und räumlicher Abdeckung entwickelt.


## Teilprojekte


### SN1 | Sensorboxen
{: #SN1 }

Team | [Bernd Freisleben]({{ site.baseurl }}{% link _about_de/0900-team.md %}#bfreisleben), [Ralf Steinmetz]({{ site.baseurl }}{% link _about_de/0900-team.md %}#rsteinmetz)
Herausforderung | Autonom kommunizierende ortsfeste und mobile Sensorboxen bilden die Datenerfassungskomponente von NatNet. Für die konkurrierenden Entwurfskriterien der Boxen bzgl. plattformspezifischen Sensorkombinationen, Gewicht, Energieeffizienz, Funkreichweite etc. (Piyare et al. 2017) müssen dedizierte Lösungen erforscht und implementiert werden.


### SN2 | Kommunikation und Apps
{: #SN2 }

Team | [Ralf Steinmetz]({{ site.baseurl }}{% link _about_de/0900-team.md %}#rsteinmetz), [Bernd Freisleben]({{ site.baseurl }}{% link _about_de/0900-team.md %}#bfreisleben)
Herausforderung | Die hochauflösenden Sensorboxen (SN1) erfordern effiziente und angepasste Kommunikationsmechanismen zur Übertragung der Daten an die zentrale Datenbank (UM1). Gleichzeitig verlangt die Mobilität und Planbarkeit der Bewegung die Realisierung von Konzepten der opportunistischen Kommunikation mittels heterogenen Funktechnologien. Bisherige Arbeiten adressieren entweder homogene Szenarien in Bezug auf die zu übertragenden Daten oder Szenarien ohne mobile Sensorplattformen (z.B. Jukan, Masip-Bruin & Amla 2017).


### SN3 | Bildungswissenschaftliche Beteiligung
{: #SN3 }

Team | [Carina Peter]({{ site.baseurl }}{% link _about_de/0900-team.md %}#cpeter)
Herausforderung | Zusätzlich zu den technischen und biotischen Plattformen bilden bürgerwissenschaftliche Aktivitäten eine zentrale Datenerfassungskomponente in NatNet. Gleichzeitig ist anzunehmen, dass durch die Einbindung von Bürgern in Forschungsaktivitäten das Wissenschaftsverständnis im Sinne einer Scientific Literacy gefördert wird. Der potenzielle Nutzen für beteiligte Bürger wurde aber bisher nicht untersucht (Bonney et al. 2009).

{% include next-previous-page-in-category content='about' %}