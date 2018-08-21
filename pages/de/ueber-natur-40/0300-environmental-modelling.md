---
subheadline: Natur 4.0 | Sensing Biodiversity
title:  "Projektbereich Umweltmodellierung"
teaser: "Ein naturschutzfachliches Monitoring in NatNet erfordert letztlich flächendeckende und zeitlich homogenisierte Datensätze, die die ökologischen Eigenschaften des Untersuchungsgebiets und die daran gebundenen Interaktionsnetzwerke abbilden. Im Projektbereich Umweltmodellierung (UM) werden hierfür operationelle Methoden zur Ableitung (klima-)ökologisch relevanter Informationen aus den heterogenen und raum-zeitlich diskontinuierlichen Datensätzen der Sensorboxen erforscht sowie räumliche Vorhersagemodelle entwickelt."
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
Im Kern des Projektbereichs UM steht die Implementierung von Modellen zum Speichern, Prozessieren und Auswerten von Sensorbox- und darüber hinaus verfügbaren Datensätzen für ein naturschutzfachliches Monitoring (Abb. 2). Die Basis bildet das analytische Datenbanksystem NatDB (UM1). Es dient als zentraler Datenspeicher und wird über definierte Schnittstellen direkt durch die beteiligten Projekte im Bereich UM schrittweise erweitert. Nutzerspezifische Analyseergebnisse und Visualisierungen werden über eine Web-Schnittstelle interaktiv bereitgestellt. Hierzu gehört auch die für die bürgerwissenschaftlichen Aktivitäten geplante Funktionalität (siehe SN3, Kap. 6.3.3). 

Mit Blick auf lokale Messungen werden in UM2 neuartige Akustik- und Radarfernerkundungsdaten zur Analyse wichtiger Elemente trophischer Netzwerke (Insekten und Vögel) entwickelt und akustische Aufnahmen auch zur integrativen Charakterisierung von Landschaften genutzt. Im Bereich der bildgebenden Verfahren werden maschinelle Lernmodelle zur Identifikation relevanter Zielgrößen (Nistplätze etc.) trainiert und Methoden zur Ableitung der Ökosystemstruktur und der Phänologie aus kostengünstigen UAV-Aufnahmen (VIS/NIR) erforscht. Für irregulär aufgenommene Variablen werden maschinelle Lernverfahren zur skalenübergreifenden räumlichen Vorhersage implementiert, die die Informationen in regulären Rasterkarten abbilden. Die Entwicklung der Modelle in UM2 erfordert verbesserte mathematische und statistische Verfahren im Bereich der Entrauschung, Signalklassifikation und Regularisierung (UM3, UM4). Hier sind insbesondere Methoden zur Detektion von Richtungsinformationen in Bilddaten oder zur simultanen Analyse von Zeit- und Frequenzräumen relevant (UM3). Verzerrung im Rahmen der Stichprobenentnahme erfordern ferner Schätzungen von Eigenschaften der Verteilungsfunktionen (UM4). Zudem werden Warnindikatoren erforscht, die die zeitliche Variabilität der Daten analysieren (UM4), wofür effiziente Datenmodelle in der NatDB implementiert werden (UM1). Die dargestellte Entwicklung und Validierung der Modelle erfolgt in enger Zusammenarbeit und in wechselnder Kombination mit den ökologischen Projektgruppen (Kap. 6.2.2). Der Projektbereich UM fungiert dabei auch als Bindeglied zwischen den Bereichen SN und ÖP. 



## Beitrag zu Natur 4.0
Der Projektbereich UM bildet die zentrale Datenvorhaltungs-, Analyse- und Modellierungskomponente von NatNet. Er liefert die für den NatNet-Prototyp notwendige Funktionalität und stellt diese über das zentrale NatDB-System zur Verfügung. Durch das Design ist die Methodik auf andere Gebiete übertragbar und der Datenaustausch mit Dritten möglich (z.B. GFBio, HLNUG, Bürgerwissenschafts-Portale). Die Modularität mit definierten Schnittstellen stellt zudem sicher, dass die Sensorboxen und Modellverfahren durch neue Entwicklungen ersetzt oder ergänzt werden können. 


## Teilprojekte


### UM1 | Datenintegration
{: #UM1 }

Projektleitung | [Bernhard Seeger]({{ site.baseurl }}{% link pages/de/team.md %}#bseeger)
Team | NN
Herausforderung | Durch das im GFBio-Projekt entwickelte VAT-System (Authmann et al. 2015) wurde bereits ein Werkzeug zur Datenintegration, Analyse und Visualisierung von Biodiversitätsdaten geschaffen, das sich ideal als Grundlage für die in diesem Projekt zu entwickelnde NatDB eignet. Es bietet Funktionalität für Import, Export, Verwaltung und Verarbeitung von Vektor- und Rasterdaten an. Daten können statisch importiert werden, eine dynamische Anbindung von Live-Daten und deren Persistierung ist in VAT derzeit aber noch nicht vorgesehen. Gleiches gilt für Bild- und Audiodaten, die zwar bereits interaktiv angezeigt, aber noch nicht verarbeitet werden können. VAT verfügt jedoch über eine Benutzer- und Projektverwaltung, die für die Erstellung von benutzerspezifischen Schnittstellen genutzt werden kann. Für die ökologische Wissenschaftsdomäne ist zudem die Interaktion mit R interessant, die sowohl im System die Einbindung von R-Funktionen als auch außerhalb den Aufruf der in VAT erzeugten Workflows in R ermöglicht. 


### UM2 | Fernerkundung und räumliche Vorhersage
{: #UM2 }

Projektleitung | [Jörg Bendix]({{ site.baseurl }}{% link pages/de/team.md %}#jbendix), [Hanna Meyer]({{ site.baseurl }}{% link pages/de/team.md %}#hmeyer), [Thomas Nauss]({{ site.baseurl }}{% link pages/de/team.md %}#tnauss), [Christoph Reudenbach]({{ site.baseurl }}{% link pages/de/team.md %}#creudenbach)
Team | NN
Herausforderung | Um konsistente, raum-zeitliche Datensätze bereitzustellen, müssen die irregulär vorliegenden Sensordaten in NatNet mit flächendeckenden, fernerkundlich erfassten Geodatensätzen verbunden werden. Die Ableitung von Ökosysteminformationen aus den heterogenen Fernerkundungsdaten erfordert dabei den Einsatz leistungsfähiger, maschineller Lernverfahren. Für das Monitoring von fliegenden Insekten und Vögeln ist ferner der Einbezug von Radar- und akustischen Informationen erforderlich. Allerdings stecken insbesondere die Radarverfahren zur mobilen Insektenerfassung noch in den Kinderschuhen und müssen auf Basis miniaturisierter Sensoren weiterentwickelt werden. 


### UM3 | Transformation, Regularisierung und Klassifikation
{: #UM3 }

Projektleitung | [Stephan Dahlke]({{ site.baseurl }}{% link pages/de/team.md %}#sdahlke)
Team | NN
Herausforderung | Im Rahmen von Natur 4.0 werden umfangreiche Datensätze unterschiedlicher Natur gesammelt und bereitgestellt. Dafür müssen sachgerechte, effiziente und verlässliche Analyseverfahren zur Extraktion der jeweils relevanten Information entwickelt werden. In Anbetracht der Größe der Datenmengen werden problemadaptierte Analyse-Verfahren, welche die strukturellen Unterschiede der verschiedenen Datentypen gezielt nutzen, im Mittelpunkt stehen.


### UM4 | Punktprozesse und Strukturbrüche
{: #UM4 }

Projektleitung | [Hajo Holzmann]({{ site.baseurl }}{% link pages/de/team.md %}#hholzmann)
Team | NN
Herausforderung | Bei aktuellen statistischen Methoden zur Ableitung von Vorkommenswahrscheinlichkeiten erfolgt die räumliche Vorhersage in der Regel durch Poissonsche Punktprozesse mit log-linearer Intensitätsfunktion in den erklärenden Variablen. Die zeitliche Variation ist für Monitoringprozesse wichtig, wird jedoch in diesen Modellen bisher nur unzureichend berücksichtigt. Insbesondere zeitliche Brüche können so nicht modelliert oder detektiert werden. Die Analyse von Fernerkundungsdaten zur Ableitung von Bestands- und Landschaftsstrukturen führt auf inverse Probleme, die derzeit in ad-hoc Verfahren mit Bayesschen Methoden gelöst werden, ohne den Grad der Regularisierung fundiert zu wählen.



{% include next-previous-page-in-category content='about' %}
