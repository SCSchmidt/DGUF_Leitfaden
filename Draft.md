---
title: Handreichung zur Rezension von Forschungssoftware - Kriterien für "gute" Forschungssoftware
layout: draft
author:
  - Anne Klammt, Deutsches Forum für Kunstgeschichte Paris
  - Timo Homburg
  - Clemens Schmid, Max-Planck-Institut für Menschheitsgeschichte Jena
  - Sophie Charlotte Schmidt
  - Lutz Schubert
  - Florian Thiery, Research Squirrel Engineers
  - Martina Trognitz, Austrian Centre for Digital Humanities and Cultural Heritage, ÖAW Wien

bibliography: literatur.bib
csl: apa-6th-edition.csl

---

<div id="zitat" markdown="1">
"Die Leitfunde werden dann im Computer durch die Programme ARCH und GGG einer Seriation unterzogen. Diese Programme entwickelte E. Kämmerer. Eine Beschreibung ist der Arbeit beigefügt. Die Programme DOK und ARCH z. Zt. für 600 Typen in 2000 Funden dimensioniert, sind am Rechner TR 440 beim Großrechenzentrum für die Wissenschaft in Berlin in Anwendung." [@goldmann_chronologische_1972, 98.](#goldmann_chronologische_1972)
</div>

---

## Gliederungsvorschlag

* [Zielsetzung](#Zielsetzung-des-Beitrags)
* [Forschungssoftware](#Forschungssoftware)
  * [Forschungssoftware als wissenschafltiche Leistung](#forschungssoftware-als-wissenschaftliche-leistung)
  * [Gute Forschungssoftware](#Gute-Forschungssoftware)
    * [FAIR-Prinzipien](#FAIR-Prinzipien)
    * [Open Science](#open-science)
    * [CARE-Prinzipien und Ethos](#care-prinzipien-und-ethos)
  * [Fachliche und technische Beurteilung](#Fachliche-und-technische-Beurteilung)
* [Anwendungsbereich dieser Handreichung](Anwendungsbereich-dieser-Handreichung) (Benötigen wir diesen Abschnitt?)
* [Vorgehensweise bei der Rezension von Software](#Vorgehensweise-bei-der-Rezension-von-Software)
* [Kriterien zur Beurteilung von Software](#Kriterien-zur-Beurteilung-von-Software)
  * ... alle Unterpunkte ab [dort](#Kriterien-zur-Beurteilung-von-Software)
* Tabellarische Zusammenfassung?

---

## Zielsetzung des Beitrags<sup>[1](#myfootnote1)</sup>
Ziel dieses Beitrags ist es Fragen und Themen aufzuwerfen, die für die Rezension von Forschungssoftware und im Forschungsprozess eingesetzten digitalen Werkzeugen relevant sind.

Die Beurteilung einer wissenschaftlichen Publikation ist eine traditionsreiche Form des wissenschaftlichen Diskurses. Entsprechend gibt es ein unausgesprochenes Verständnis davon, was eine gute Rezension ausmacht. Unterstützt werden kann dies durch redaktionelle Maßnahmen zur Qualitätssicherung wie Hinweise für die/den Rezensentin/Rezensenten oder - wie es die DGUF mit den Archäologischen Informationen praktiziert - eines Reviews der angefertigten Rezension. Die Frage ist jedoch, was sollte eine gute Rezension von Software für den Einsatz in der Archäologie ausmachen? Geht es dabei allein um Aspekte der Nutzbarkeit, der Usability? Sollten nicht auch Fragen der Nachhaltigkeit und der Anschlussfähigkeit einfließen? Müsste nicht auch betrachtet werden, ob es eine wissenschaftliche Dokumentation und Diskussion der rechnerischen Verfahren gibt - etwa bei den vielen Interpolationen von Daten mit Raumbezug, die moderne GIS-Softwarepakete bieten?

In dieser Handreichung erläutern wir einige Kriterien für gute Forschungssoftware. Dabei folgen wir den Empfehlungen der DFG und weisen auf sogenannte "open standards" hin. Software greift im- und explizit tief in den Forschungsprozess ein (für die Archäologie siehe z.B. [@schmidt_marwick_2020](#schmidt_marwick_2020)) und nur durch die Offenlegung von Quellcode ist eine Bewertbarkeit der durch die Software geleisteten Abläufe gewährleistet.

Wir empfehlen eine Vorgehensweise zur Softwarerezension und sammeln Kriterien, die für die Bewertung einer Software von Bedeutung sein können. Aufgrund der Vielfalt der möglichen Besprechungsgegenstände werden nicht in jedem Fall alle Kriterien von Bedeutung sein.

Die hier vorgestellten Überlegungen, Kriterien und Vorschläge sollen den Rezensentinnen und Rezensenten als Arbeitserleichterung dienen. Diskussionsbeiträge sowie Anregungen zu diesen Beitrag sind erwünscht. Dazu können entweder die Autoren kontaktiert werden oder -- hier website (https://research-squirrel-engineers.github.io/DGUF_Leitfaden/) und Kontaktdaten einfügen ? -- genutzt werden.

## Forschungssoftware

Die weiter unten vorgestellten Kriterien zur Rezension von Software zielen primär auf die Begutachtung von Forschungssoftware ab. Unter Forschungssoftware verstehen wir Software, `die mit Fokus auf einen Einsatz in der Forschung entwickelt wurde`, also um Forschungsdaten zu erzeugen, zu verarbeiten oder zu analysieren [@hettrick_2014_14809](#hettrick_2014_14809). Dies sind beispielsweise Programme, die der Kalibrierung und Umrechnung von Messwerten, der Annotation von Texten und Objekten, oder der Bereitstellung sowie der Verknüpfung und Visualisierung fachlich relevanter Vokabulare dienen.

Forschungssoftware kann entweder für einen sehr spezifischen Bedarf oder einen allgemeinen Anwendungsbereich entwickelt worden. Sie ist dabei stets Teil des Forschungsprozesses, der in allen seinen Punkten nachvollziehbar und soweit möglich reproduzierbar sein muss.

Im Gegensatz zu Forschungssoftware steht Software, die zur Nutzung spezifischer Geräte erforderlich ist, wie etwa zur Vermessung, zur fotografischen Dokumentation oder zur Analyse von Oberflächen und Inhaltsstoffen. Häufig handelt es sich um proprietäre Software, die zusammen mit der Hardware vertrieben wird. Obwohl sie im Forschungsprozess eingesetzt wird, entspricht sie nicht unserem Verständnis von Forschungssoftware. Auch digitale Werkzeuge, die eine erhebliche Rolle in der praktischen Arbeit inne haben, jedoch keinen eigentlichen Anteil an der Erhebung, Bearbeitung und Analyse der Daten haben, sind in unserem Sinne keine Forschungssoftware. Trotzdem können auch diese Tools mittels der vorgestellten Kriterien beurteilt werden.

Forschungssoftware ist in besonderer Weise Herausforderungen nachhaltiger Entwicklung und Pflege ausgesetzt. Ein Hauptfaktor für mangelnde Nachhaltigkeit von Forschungssoftware ist der Mangel an langfristiger Finanzierung für `Forschungssoftware-Ingenieure`, die sich um die geeignete Architektur, Organisation, Implementierung, Dokumentation und Interaktion mit der Gemeinschaft für die Software kümmern, gepaart mit der Umsetzung von Maßnahmen, um die Software während und nach dem Entwicklungsprozess nachhaltig zu machen ([@anzt_environment_2020, 2](#anzt_environment_2020)). Einen Überblick über Bedarfe, Herausforderungen und Lösungsansätze zu Förderung und Finanzierund, Selektion, rechtliche Fragen, Organsiation und Governance, sowie Bündelung von Ressourcen wurden in einem Workshop der deRSE Konferenz in Potsdam 2019 entwickelt ([@bach_dersews19](#bach_dersews19)).

### Forschungssoftware als wissenschaftliche Leistung

In der modernen Forschung ist ein Arbeiten ohne digitale Werkzeuge undenkbar. Dies trifft ebenfalls auf die historische und altertumswissenschaftliche Forschung zu. Mit dem Aufschwung der Digital Humanities wird Forschungssoftware weiterhin und auch zunehmend ein wichtiger Bestandteil des Forschungsprozesses sein.

Trotz der tragenden Rolle, die Forschungssoftware in manch einem Projekt hat, wird die Leistung der Personen, die hinter der Entwicklung und Programmierung stehen, akademisch nicht anerkannt ([@hettrick_2017](#hettrick_2017), [@scheliga_pampel_2017](#scheliga_pampel_2017) und [@katerbow_2018](#katerbow_2018)). Jedoch fließen einerseits bei der Entwicklung von Forschungssoftware teilweise jahrelange technische Erfahrung und Praxis ein. Andererseits wird aber auch Wissen über wissenschaftliche Standards und Praktiken angewendet. Durch die Umsetzung in Code wird Praxis und Wissen explizit gemacht und weiterentwickelt. Diese Leistungen gilt es zu würdigen und sichtbar zu machen ([@scheliga_pampel_2017](#scheliga_pampel_2017), [@katerbow_2018](#katerbow_2018) sowie [@helmholtz_web](#helmholtz_web)).

Als erster Schritt in Richtung Sichtbarmachung wurde 2012 die Berufsbezeichnung des "Software Research Engineers" (RSE, RSEng) geprägt ([@hettrick_2017](#hettrick_2017) und [@baxter_2012](#baxter_2012)). Mittlerweile hat sich auch eine aktive, internationale und interdisziplinäre Gemeinschaft gebildet, die unter anderem auch in Deutschland als de-RSE e.V. tätig ist, Konferenzen organisiert und Empfehlungen gibt ([@anzt_environment_2020](#anzt_environment_2020)). Auch im internationalen Kontext entwickeln sich immer mehr nationale [RSE Sektionen](https://sorse.github.io/contact/chapters/) und gemeinsam von der RSE Community organisierte Konferenzen, wie z.B. [SORSE](https://sorse.github.io). Im Rahmen des Aufbaus einer `Nationalen Forschungsdateninfrastruktur (NFDI)` nehmen Forschungssoftware und RSEs einen großen Stellenwert in der wissenchaftlichen Praxis ein ([@loeffler_nfdi4rse20](#loeffler_nfdi4rse20) und [@goedicke_nfdixcs20](#goedicke_nfdixcs20)).

Eine der Forderungen der de-RSE e.V. ist, dass Forschungssoftware mittels geeigneten Publikationsmodalitäten sichtbar gemacht werden soll, da ein Publikation und vor allem deren Auffindbarkeit redundante Arbeit vermeidet ([@anzt_environment_2020, 10](#anzt_environment_2020)). Dabei ist die eindeutige Autorenschaft von großer Bedeutung, da erst dadurch die Leistung der Forschungssoftwareentwicklung an die entsprechenden Personen geknüpft werden. Dies eröffnet akademische Karrierewege, in denen bislang nur klassische Publikationen gewertet wurden. Zukünftig sollten aber in gleicher Weise auch Datenpublikationen, Softwareentwicklung und -publikationen (https://citation-file-format.github.io, https://doi.org/10.5281/zenodo.1003149), Annotationen, sowie deren Zitationen als Kriterien der Beurteilung der wissenschaftlichen Leistung sein (s. NFDI4Culture, RSE4NFDI, NFDI4Objects).

Ein Beispiel für die Nennung der Autorschaft bildet das einleitende Zitat, das die Erfahrungen der Archäologischen Informationen widerspiegelt. Allerdings gibt es grundlegende Unterschiede zu gewohnten Publikation von Aufsätzen und Büchern. Da die Entwicklung von Software auf bereits bestehenden Modulen aufbaut, muss das Verständnis von Autorenschaft und wie sie sich auch über die Lebenszeit der Software hinaus dokumentieren lässt spezifisch für Software erfolgen [@katz_software_2016](#katz_software_2016).

Eine publizierte Software kann anschließend, ganz so wie in der bisherigen Praxis der altertumswissenschaftlichen Forschung, begutachtet werden. In einer Rezension kann diese dann einem breiteren Publikum vorgestellt werden. Mit der Einführung der Rezensionskategorie "Archäoinformatik" intendiert die Redaktion der Archäologischen Informationen genau dies. Durch eine dedizierte Rezension von Software analog zu Rezensionen wissenschaftlicher Publikationen, wird die wissenschaftliche Leistung der Autoren und Autorinnen von Forschungssoftware mittels gewohnten Formaten sichtbar und anerkannt.

### Gute Forschungssoftware

Um überhaupt Kriterien zur Rezension und Bewertung von Forschungssoftware aufstellen zu können, stellt sich zunächst die Frage was überhaupt eine gute und modernen Standards entsprechende Forschungssoftware ausmacht.

Da die Software ein integraler Bestandteil des Forschungsprozesses ist, gelten zunächst die "Leitlinien zur Sicherung guter wissenschaftlicher Praxis", wie sie die DFG ([@deutsche_forschungsgemeinschaft_2019](#deutsche_forschungsgemeinschaft_2019)) fordert. Allein hieraus ergeben sich schon wichtige Anforderungen wie die Einhaltung und Etablierung von Standards und Methoden, eine nachvollziehbare Dokumentation des Weges zu den Ergebnissen sowie der öffentlicher Zugang der Ergebnisse und die Archivierung der Materialien die zu einem Forschungsergebnis geführt haben.

Wir möchten auf ein paar der Aspekte, die sich aus den DFG-Leitlinien ergeben, näher eingehen. Sie entsprechen dem internationalen Konsens und etablierten Prinzipien: die in der Erläuterung zu Leitlinie 13 - Herstellung von öffentlichem Zugang zu Forschungsergebnissen - genannten FAIR-Prinzipien, sowie die Prinzipien der Offenen Wissenschaft (Open Science). Außerdem sollen die CARE-Prinzipien, welche in den Leitlinien 2 und 10 der DFG anklingen, erläutert werden. Hinweise zur Umsetzung der DFG-Leitlinien in Bezug auf Forschungssoftware sind unter [@forschungsdaten_info_dfg](#forschungsdaten_info_dfg) zu finden.

#### FAIR-Prinzipien
Die FAIR-Prinzipien wurden 2016 als FAIR Data Principles veröffentlicht [@wilkinson_2016](#wilkinson_2016). Sie zielen primär auf Forschungsdaten und deren Metadaten ab und fordern dass diese auffindbar (Findable), zugänglich (Accessible), interoperabel (Interoperable) und nachnutzbar (Reusable) sind. Die Prinzipien können auch auf Forschungssoftware und deren Metadaten übertragen werden ([@lamprecht_towards_2019](#lamprecht_towards_2019), [@goedicke_2020](#goedicke_2020)).

Die Anwendung von FAIR-Prinzipien fördert die Qualität der Software hinsichtlich der grundsätzlichen Ansprüche an Interoperabilität bei der Verwendung in einem Workflow und der Verwendung von Standards und etablierten Paradigmen des Programmierens und der Dokumentation. Die FAIR-Prinzipien beziehen sich nicht auf die wissenschaftliche Qualität des Tools. Dennoch ergeben sich eine Anzahl von Kritertien, die in die Beurteilung einer Forschungssoftware einfließen und von Angaben, die im Rahmen der Rezension als Serviceleistung zu erbringen sind, wie die Autorenschaft, das zur Speicherung verwendete Repositorium oder mögliche nötige Voraussetzungen zur Verwendbarkeit.

Ein Fokus der FAIR-Prinzipien ist, dass Daten, bzw. Forschungssoftware, und Metadaten auch maschinell lesbar und verarbeitbar sind. Dies betrifft vor allem die Prinzipien 'Accessible' und 'Interoperable'.

##### Findable (Auffindbar)

Software wird durch die Speicherung zusammen mit ihren Metadaten in dedizierten Softwarerepositorien auffindbar, welche kommerziell, community-basiert und in vielen weiteren Formen starke Impulse für die Entwicklung der wissenschaftlichen Infrastrukturen geben. Die Auffindbarkeit wird durch die fachwissenschaftliche Einbindung und die klassische Arbeit von Forschungsinfrastrukturen zusätzlich erhöht, da sie Aufbau, Pflege und Anwendung von kontrolliertem Vokabular und Metadatenstandards zur Indexierung betreiben ([@lamprecht_towards_2019](#lamprecht_towards_2019) und [@anzt_environment_2020, 10](#anzt_environment_2020)).

Die Vergabe von persistenten URLs durch Repositorien, sowie die Nennung der Autorenschaft ermöglicht das Zitieren von Forschungssoftware. Wichtig ist hierbei, dass Software, da sie im Gegensatz zu herkömmlichen Publikationen kontinuierlich weiterentwickelt wird, in unterschiedlichen Entwicklungsständen abgelegt wird, damit bestimmte Versionen zitiert werden können [@forschungsdaten_info_dfg](#forschungsdaten_info_dfg).


##### Accessible (Zugänglich)

Entsprechend den FAIR-Prinzipien sollte Software und die sie beschreibenden Metadaten über ihre persistente URL erreichbar sein. Dies sollte auch maschinell über ein offenes und standardisierte Kommunikationsprotokoll möglich sein [@lamprecht_towards_2019](#lamprecht_towards_2019).

Weitere Aspekte, welche die Zugänglichkeit erleichtern, sind die Verfügbarkeit für verschiedene Betriebssysteme, sowie technische Anforderungen welche von aktuell verbreiteten Geräten geleistet werden können. Eine verständliche Anleitung zur Nutzung des Programms verbessert die Zugänglichkeit im Sinne der Nutzbarkeit.

> [MT] 'kostenlos' entfernt. FAIR fordert das nicht. Wir könnten aber 'Kosten' als Kriterium einfügen

##### Interoperable (Interoperabel)

Interoperabilität von Software kann sich zum Einen auf die Kompatibilität der Ein- und Ausgabeformate mit anderen Programmen in einem Arbeitsprozess (horizontale Dimension) beziehen. Zum Anderen verweist sie auch auf die Zusammenarbeit der verwendeten Komponenten in der Software selbst (vertikale Dimension) [@lamprecht_towards_2019, 46 f.](#lamprecht_towards_2019). Beides wird durch die Verwendung von Standards ermöglicht, welche eine Installation von Software auf unterschiedlichen Betriebssystemen ermöglichen.


##### Reusable (Nachnutzbar)

Die Nachnutzbarkeit von Software hängt von mehreren Komponenten ab. Die Metadaten und eine umfassende Dokumentation der Software sollten es anderen ermöglichen Ergebnisse zu reproduzieren, sowie eigene Daten und veränderte Anwendungsfälle zu prozessieren. Eine geeignete Lizenz, welche auch die abhängigen Softwarekomponenten berücksichtigt gibt zudem darüber Auskunft welche Regeln bei der Nutzung gelten und ob eine Weiterentwicklung des Codes möglich ist. Für die Zitierbarkeit ist eine Nennung der Beteiligten notwendig [@lamprecht_towards_2019, 48-49](#lamprecht_towards_2019).


#### Open Science

Open Science (Offene Wissenschaft) bezeichnet eine Wissenschaftspraxis, deren Ziel ein transparenter, replizierbarer und kollaborativer Forschungsprozess ist [@bezjak_openscience_2018, Open Concepts and Principles](#bezjak_openscience_2018). Open Science setzt sich aus mehreren Prinzipien zusammen, die unterschiedliche Stadien im Forschungsprozess betreffen.

So fordert Open Science nicht nur die Öffnung der Ergebnisse (Open Access), sondern auch der zugrundeliegenden Daten (Open Data), Methoden (Open Methodology) und der verwendeten Forschungssoftware (Open Source). Für offene Forschungssoftware gilt, dass ihr Quellcode zugänglich und mit einer Lizenz versehen sein muss, welche die Weiterentwicklung erlaubt [@bezjak_openscience_2018, Open Research Software and Open Source](#bezjak_openscience_2018).

In den Leitlinien der DFG klingt die Öffnung von Software-Quellcode im Zusammenhang mit der Qualitätssicherung [@deutsche_forschungsgemeinschaft_2019, 14-15](#deutsche_forschungsgemeinschaft_2019) und der Herstellung von öffentlichem Zugang zu Forschungsergebnissen [@deutsche_forschungsgemeinschaft_2019, 19](#deutsche_forschungsgemeinschaft_2019) an.

Mit der Forderung nach der Offenlegung des Quellcodes (Open Source), wird auch dem Gedanken der Nachnutzbarkeit entsprochen. Die Offenlegung wird erweitert um die Forderung, den Code zudem frei nutzbar zur Verfügung zu stellen (Free Source). Letzteres wird als FOSS (Free/Libre Open Source Software) bezeichnet und wird in Deutschland z.B. von anwendungsbezogenen Wissenschaftler\*innen und Entwickler\*innen aus der Geoinformatik vertreten (FOSSGIS e.V.). oder von Research-Software-Engineers in der "de-RSE e.V." [@anzt_environment_2020](#anzt_environment_2020).


#### CARE-Prinzipien und Ethos

In den Leitlinien der DFG werden in Leitline 2 und 10 ethische Aspekte im Forschungsprozess angesprochen, die auch im Bereich der Forschungssoftware Beachtung finden sollten.

Forschungssoftware ist nicht neutral. Sie entsteht nicht unter neutralen Bedingungen, ihre Nutzung erfolgt unter spezifischen Voraussetzungen und auch ihre Weitergabe unterliegt den vorherrschenden Konventionen und Gewohnheiten. Vielfach tragen diese Gewohnheiten und Konventionen zur (unbewussten) Festigung von Privilegien und Diskriminierungen bei, etwa wenn Tutorials ausschließlich männliche Nutzer kennen, oder die an der Entwicklung beteiligten Personen nicht genannt werden.

Wie angemessen ist es beispielsweise, wenn für die archäologische Feldarbeit Software zur Datenaufnahme eingesetzt wird, welche für die Mehrheit der Mitarbeiter\*innen vor Ort aufgrund einer Sprachbarriere nicht verständlich ist? Diskriminiert freie und offen lizensierte Software, die aber für ihre Verwendung proprietäre Software oder teure Hardware voraussetzt Forscher und Forscherinnen mit weniger Finanzmitteln?

Dass Software Gruppen und Individuen diskriminieren kann, zeigen entsprechende Untersuchungen, wie etwa der Fall von Facial-Recognition-Software, die ausschließlich auf die Erkennung hellhäutiger Menschen geeicht ist [@breland_how_2017](#breland_how_2017). Auch für diese kritische Auseinandersetzung mit Forschungssoftware sollte deren Autorenschaft zuweisbar gemacht werden. 

Gerade in den Altertumswissenschaften, in denen häufig an fremden Kulturen und Kulturhinterlassenschaften geforscht wird, sollten die Rechte der indigenen und einheimischen Bevölkerung bezüglich ihres kulturellen Erbes und des damit zusammenhängenden Wissens berücksichtigt werden. Hierfür eignen sich die CARE-Prinzipien (https://www.gida-global.org/care). Sie wurden von der Global Indigenous Data Alliance (GIDA) und der Research Data Alliance (RDA) 2018 auf Basis der UN Declaration on the Rights of Indigenous Peoples (UNDRIP) erarbeitet.

Das CARE-Akronym steht für folgende vier Prinzipien, welche auch bei der Entwicklung von Forschungssoftware Beachtung finden sollten:

> [MT] hier könnte man nach jedem Prinzip eventuell in ein, zwei Sätzen die Relevanz für Software hervorzuheben

- **C**ollective Benefit: Dieser Punkt fordert den gemeinschaftlichen Nutzen der Datenerhebung für die indigene Bevölkerung. Er lässt sich leicht auf Software übertragen: Software, die auf Wissen und Erfahrungen von indigenen Bevölkerungen beruht, soll für diese Gruppen einen Nutzen haben. Hier geht es darum, dass Menschen, die einen wichtigen Beitrag für die Entwicklung geleistet haben, honoriert werden und die Anwendung nicht nur Fremden zugute kommt (monetär, durch Reputation u.ä.). 

- **A**uthority to Control: Die Kontrollmacht über die eigenen Daten ist eine wichtige Forderung Indigener Menschen. Auch dies lässt sich auf Software anwenden: Die Entscheidungsmacht über die Verwendung von anhand ihres Wissens entwickelter Software soll bei der Indigenen Bevölkerung liegen. Dieser Punkt kann verhindern, dass indigenes Wissen unangemessen ausgenutzt wird und kann durch die computertechnische Ermächtigung von Indigenen verstärkt werden.

- **R**esponsibility: Wer mit Indigenen Daten arbeitet, hat die Verantwortung nachvollziehbar aufzuzeigen, wie diese Daten den Indigenen Gruppen zugute kommen. Entwickler von Software haben Verantwortung für die positive Folgen der Software für die Indigenen Gruppen zu übernehmen. Bei der Entwicklung ist es die Verantwortung der Produzenten mögliche schädliche Konsequenzen der Software auszumerzen. Dies kann durch inklusve Ansätze bei der Entwicklung verfolgt werden.

- **E**thics: Rechte und Wohl der indigenen Bevölkerung sollten an erster Stelle bei der Erarbeitung und Bearbeitung eines Datensatzes stehen. Für Software gilt das gleiche, wenn sie indigene Völker betrifft. 

> [SCS] muss nochmal auf angemessene Sprache geprüft werden (Indigene oder indigene wird zB im englischsprachigen diskutiert. "Bevölkerungen" oder "Völker" etc)


## Fachliche und technische Beurteilung

Die genannten Prinzipien rund um FAIR, Open Science und CARE dienen vor allem der allgemeinen Bewertung von Software. Jedoch werden noch eine Reihe fachliche und technische Spezifika benötigt, um in einer Rezension die Leistung der Entwickler\*innen angemessen zu beurteilen.

> [MT] die folgenden Teile in diesem Abschnitt gehören noch überarbeitet
> [SCS] besser?

Die Beschäftigung mit der wissenschaftlichen Nutzung, also den Nutzungsszenarien von Forschungssoftware, ist in der archäologischen Forschung bereits verankert (bezogen auf die Ur- und Frühgeschichte und die Archäologie des Mittelalters). Die AG CAA e.V. führt seit 2010 jährlich Workshops durch, in denen Tutorials zu Software durchgeführt und Fallbeispiele diskutiert werden sowie Entwickler\*innen ihre Tools zur Diskussion stellen. Auch in den Fachzeitschriften und Tagungen mit anderen thematischen, räumlichen und zeitlichen Schwerpunkten werden in gewisser Regelmäßigkeit entsprechende Fallbeispiele publiziert. Tagungen, Sammelbände uns Ausstellungen nehmen sich bestimmter Themen an, wie der Auswertung von LIDAR-Daten oder 3D-Rekonstruktionen (LIT./LIT).

Die Publikationen von Forschungsergebnissen, die unter dem Einsatz spezifischer Forschungssoftware erzielt wurden, legen je nach Qualität der Arbeit die zugrundeliegenden Berechnungswege, die Modellierung der Daten und die Wechselbeziehung mit dem Forschungsdesign dar (exemplarisch: Zimmermann, Saile, Freund). Eine insgesamt kleinere Anzahl von Autorinnen und Autoren setzen sich in ihren Beiträgen explizit mit der Leistungsfähigkeit und den Parametern dieser Rechnungen selbst, bzw. den Algorithmen auseinander (exemplarisch: Irmela Herzog 2012, 2014 und Gerhard Roth LIT). Diese, aus der eigenen fachlichen Traditionen der Archäologie entwickelten, Kriterien sind für die Rezension einer Forschungssoftware ebenfalls für Bedeutung, da sie das Potenzial für die wissenschaftliche Arbeit und die Passung zum Forschungsfeld beschreiben.


##  Anwendungsbereich dieser Handreichung

> [MT] Die Absätze hier sind irgendwie übrig geblieben und so ganz passen sie nicht zur Überschrift. Entweder streichen oder bei den jeweiligen Kriterien mit einbauen
> Evtl. wird dieser Abschnitt auch nicht benötigt
> [SCS] m.E. kann er weg

Hardwarespezifische Software
, aber ihre Programmierung ist nicht transparent, vielfach werden zudem Daten in proprietären Formaten erzeugt. Entsprechend können zwar der Umgang mit der Software und die Produktqualität aus Sicht der Nutzerinnen als Erfahrungswerte beschrieben werden, aber es können keine begründeten Aussagen zur Performanz unter veränderten Bedingungen, zur Stabilität und anderes getroffen werden. Einige der im folgenden dargestellten Kriterien zur Rezension von Forschungssoftware können somit auf proprietäre Software angewendet werden und eine Berücksichtigung der Aspekte wird ausdrücklich empfohlen.

Weitere digitale Werkzeuge (*tools*)
 Ihre Passgenauigkeit setzt wie bei der eigentlichen Forschungssoftware eine genaue Kenntnis des Arbeitsfelds voraus und entsprechend sind nicht selten stehen die eigenen Kolleg\*innen hinter der Entwicklung. Eine angemessene Besprechung der Software kann hier sehr direkt zur Verbesserung des Tools führen.


## Vorgehensweise bei der Rezension von Software

In Vorbereitung zur Formulierung einer Softwarerezension ist es angemessen, zunächst möglichst ihre gesamte Dokumentation zumindest zu visitieren. Das kann Webseiten, Handbücher und wissenschaftliche Publikationen einschließen. Sofern es nicht ohnehin schon erfolgt ist, sollte die Software installiert und mit für sie typischen Testszenarien konfrontiert werden. Das heißt, die oder der Rezensent\*In sollte die Software selbst erprobt haben. Zuletzt ist ein Blick in den Programmcode -- sofern offen verfügbar -- sinnvoll.
>[SCS], wenn der Rezensent\*In in der Lage ist, ihn zu begutachten.

Der Rezensionstext sollte wie die Besprechung einer Publikation zunächst mit einer kurzen, überblicksartigen Beschreibung der Software beginnen. Zusammengefasst vorgestellt werden sollte ihr Einsatzbereich, ihre Komponenten und ihr Entstehungskontext. Für die anschließende detaillierte Besprechung und Einschätzung möchten wir die unten folgenden Kriterien vorschlagen. Diese Kriterien sind konkrete Ableitungen aus den eingangs abstrakt erläuterten Prinzipien und Anforderungen an Forschungssoftware. Nicht allen Kriterien kann und muss das selbe Gewicht zukommen - es ist der oder dem Rezensent*In überlassen Schwerpunkte zu setzen. Zuletzt sollten die Ergebnisse der Betrachtung in einer Stellungnahme zusammengefasst werden, die die Software hinsichtlich ihrer Nützlichkeit, ihrer Bedienbarkeit, ihrer handwerklichen Qualität und ihrer Position in Relation zu den Idealen guter Forschungssoftware (z.B. FAIR und CARE), beurteilt.

Der Umfang der Rezension sollte 1000-2000 Worte nicht übersteigen.

## Kriterien zur Beurteilung von Software

Im folgenden stellen wir einen Katalog von Kriterien vor, die für die Beurteilung wissenschaftlicher Software relevant sein können. Er ist weder vollständig noch au­to­ri­ta­tiv. Nicht jeder gelistete Aspekt ist für jede Software relevant und gegebenenfalls ist es nicht möglich, die entsprechende Information abzufragen oder eine gewählte Lösung zu beurteilen.

### Wissenschaftliche Relevanz und Korrektheit

Wissenschaftliche Software ist nur dann gut, wenn sie einen konkreten Zweck verfolgt und ihre Aufgabe (im wesentlichen) korrekt erfüllt. Tut sie das nicht, so sind alle weiteren Beurteilungskriterien hinfällig. Die Frage der Relevanz sollte für eine archäologische Softwarerezension auf die speziellen Bedingungen und Erfordernisse des Faches Rücksicht nehmen. Demgegenüber mitunter deutlich schwieriger zu beurteilen ist die Korrektheit der Ergebnisse einer Software. Dieses Problem gliedert sich in mehrere Aspekte: Zunächst stellt sich die sehr technische Frage, ob die in der Dokumentation genannten Algorithmen fehlerfrei in Programmcode ausgedrückt wurden. Meist ist schon eine Prüfung dieses Aspekts nicht trivial und übersteigt den Rahmen einer Rezension. Darüber hinaus versprechen wissenschaftliche Softwarewerkzeuge implizit oder explizit, die Beantwortung wissenschaftlicher Fragestellungen zu ermöglichen oder zumindest zu vereinfachen. Eine GIS-Applikation zur Analyse von Punktmustern kann etwa für den Zweck konzipiert sein menschliches Siedlungsverhalten nachherzusagen. Die Frage, ob der Algorithmus dazu semantisch überhaupt in der Lage ist, kann den Umfang einer Rezension bei weitem übersteigen und muss gegebenenfalls mit einer kritischen Benennung der Problemstellung übergangen werden.

#### Einsatzgebiet und Relevanz
* Welches Problem versucht die Software zu lösen bzw. welche Aufgaben werden mittels der Software bei der Erfassung, der Verarbeitung oder der Analyse durchgeführt. Wie sind diese Probleme und Aufgaben von ihrer Relevanz und von ihrer Häufigkeit einzuschätzen?
* Wie löst die Software das gegebene Problem? Wie ist die grundsätzliche Funktionsweise konzipiert? Was sind die wesentlichen Bestandteile in Frontend und Backend (z.B. WebApp + Datenbank, CLI + Neuronales Netz, ...)?
* Wie funktioniert der (wissenschaftliche) Algorithmus, der mit der Software implementiert wurde (natürlich in kurzen Worten: Punktmuster gehen hinein, Magie passiert, Kennwerte kommen heraus)?
* Gibt es neben der Software noch weitere Alternativen, oder ist sie die einzige für diesen spezifischen Einsatzbereich?
* Wenn es Alternativen gibt: In welchen wissenschaftlichen und technischen Eigenschaften unterscheiden sie sich?
* Entspricht der archäologische Einsatz den generellen Anwendungszenarien, den die Entwickler\*innen vor Augen hatten?
* Wie ist die Software publiziert und verfügbar (Download, git) und ist sie zitierbar (Zenodo, [CCF](https://citation-file-format.github.io)), also für die wissenschaftliche Verwendung geeignet?

#### Korrektheit der Implementierung
* Sind die Algorithmen korrekt implementiert worden?
* Ist das wissenschaftliche Ergebnis jenseits aller technischen Unterschiede vergleichbar zu anderen Implementierungen/Tools
* Ist die Behauptung, eine bestimmte wissenschaftliche Fragestellung mit gewähltem Algorithmus lösen zu können, korrekt?

### Bedienbarkeit

Die Bedienbarkeit von Software ist von zentraler Bedeutung, da sie als Flaschenhals zwischen realer und digitaler Welt alle Interaktion zwischen Nutzer und Software determiniert. Sie ist damit auch ein wichtiger Indikator für die Qualität des zugrundeliegenden Software Engineering. Letzteres ist eine "handwerkliche" Kompetenz und ein Meister des Faches orientiert sich an Ergebnisse aus langjähriger Forschung zu idealem Interfacedesign (Zitat!). Ähnlich wie bei handwerklichen Produkten ist die Qualität des gesamten Produkts für die Endnutzer\*innen also bis zu einem gewissen Grad an der Nutzeroberfläche erkennbar -- freilich mit vielen unrühmlichen Ausnahmen. Über Installation, Interface und Maschinenschnittstellen hinaus, sind auch Hilfefunktionen und die Größe und Aktivität der Nutzercommunity entscheidend für die praktische Bedienbarkeit. Gerade letzteres ist nicht zuletzt für die Zukunftsfähigkeit und damit die Eignung für den Einsatz auf institutioneller Ebene und in langfristigen Vorhaben von nicht zu unterschätzender Wichtigkeit.

Die folgenden technischen Merkmale sind Kriterien, die die Benutzbarkeit (Usability) betreffen. Weitere technische Merkmale aus einer eher Entwickler-zentrierten Perspektive betrachten wir weiter unten.

#### Installation, Lizenzierung, Laufzeitverhalten
Obwohl die meiste Software inzwischen mit Installationsskripten ausgeliefert wird, die fast alle Schritte automatisieren, sind einige Anwendungen - vor allem aus dem Open Source und Private Sektor - nur als source code verfügbar, die selbst compiliert werden müssen. Dies erlaubt nur geschulten Personen, die Anwendung zum Laufen zu bringen, dafür können mehr Endgeräte damit bedient werden und Erweiterungen selber vorgenommen werden. Idealerweise wird ein Spektrum an Möglichkeiten angeboten, doch dies bedeutet zusätzlichen Aufwand für den Entwickler und wird deswegen zumeist nicht angeboten. Stattdessen stellt sich die Frage direkt an die IT Experte des Nutzers. Man muss dabei beachten, dass mehr und mehr Anwendungen web-basiert angeboten werden und damit Plattform-unabhängig(er) sind. Solche Anwendungen sind zumeist dann allerdings an eine (stabile) Netzanbindung gebunden, was gerade auf Ausgrabungen selten gegeben ist. Software, die dennoch offline nutzbarist, ist noch verhältnismäßig selten, wird aber in Zukunft zunehmen. 
Für die Nutzer ist daher wichtig, von vorneherein zu wissen, auf wie viele Herausforderungen sie sich nlassen müssen, alleine um die Anwendung stabil zum Laufen zu kriegen. Insbesondere professionelle Anwendungen kommen mit einer klaren Liste von Spezifikationen, die sich an die ausführende Hardware und das Betriebssystem stellen um die Anwendung nutzen zu können - dieses Kriterium wird jedoch bei Open Source weniger häufig erfüllt. Idealerweise stellt eine Rezension solche Informationen zur Verfügung - wo vorhanden durch Verweis auf die angegebenen Spezifikationen und wo nicht vorhanden, so zumindest auf Basis des Kenntnisstandes des Benutzers. Dabei sollten die Rezensenten auf die eigene Umgebung verweisen und Erfahrung bei Installation und Ausführung der Software in diesem Kontext erläutern.

#### Interface
Nutzbarkeit ist stark bestimmt durch die Software-Oberfläche (UI) - diese mag in manchen Fällen graphisch gestützt sein, in anderen Fällen rein kommando-basiert sein. Die Komplexität der Oberfälche mag dabei für viele Nutzer ein No-Go-Kriterium sein und weite Forschungsfelder beschäftigen sich allein mit der Fragestellung, welche Benutzerführung intuitiv nachvollziehbar ist. Viele Faktoren spielen dabei eine Rolle, angefangen mit Gewöhnung an verschiedene, weit verbreitete Oberflächen-Gestaltungen, wie z.B. Windows gegenüber MAC OS, die jeweils einer anderen Philosophie folgen; aber auch kulturelle Faktoren spielen dabei eine große Rolle, wie alleine schon die Menü- und Text-Orientierung von links nach rechts.
Die Bewertung der Benutzbarkeit der Oberfläche ist daher ein stark subjektives Kriterium, welches jedoche einige objektive(re) Aspekte mit sich bringen. So sind z.B. Verständlichkeit der Menü-Einträge oder der Kommandos, aber auch die Aussagekraft von Fehlermeldungen und die Bereitstellung einer ausführlichen Hilfe-Seite alles Aspekte die in der Rezension kritisch beugtachtet werden sollten. Barrierefreiheit ist bei Software noch leider ein unzureichend abgedecktes Kriterium, welches allerdings zunehmend Beachtung findet und daher in der Begutachtung berücksichtigt werden sollte. Da die Oberfläche einen hohen Entwicklungsaufwand darstellt, sollte die Kritik relativ zu Kosten und Nutzerspektrum erfolgen: an eine professionelle Software mit 1.000€ Lizenzgebühren darf sicher höhere Ansprüche gestellt werden, als an ein freies R-Paket. Um das subjektive Kriterium abzudecken, ist zudem empfehlenswert, dass die Rezensenten diese auch subjektiv anführen, um dem Leser ein eigenes Bild zu erlauben.

#### Interoperabilität
Für viele Nutzer spielen Datenformate eine große Rolle, da diese die Kompatibilität zu anderen Anwendungen bestimmt. Dies betrifft sowohl, welche Datenformate gelesen, als auch geschrieben werden können. Leider ist das Spektrum an proprietären Formaten auch bei Standard-Software groß und eine Anforderung an volle Kompatibilität sollte aus praktischen Gründen nie gestellt werden, geschweige denn, dass dieser von Rezensenten komplett erfasst werden könnte. Bei vielen Anwendungen werden die unterstützten Dateiformate allein durch den entsprechenden Menü-Eintrag klar und es ist hilfreich, im Rahmen einer Renzension diesen - soweit bekannt - anzuführen, so dass potenzielle Anwender die Kompatibilität zu ihren Anwendungen prüfen können.

#### Zugänglichkeit, Hilfefunktionen und Community
* Wo finde ich mehr Informationen zu dieser Software? Hyperlinks und Referenzen.
* Gibt es Anwendungsbeispiele der Software, ggf. Beispieldatensets und eine Anleitung für diese um ein Verständnis für die Funktionsweise zu entwickeln?
* Wird es dem Benutzer einfach gemacht die Software zu testen? Gibt es eine VM, einen Dockercontainer, einen Installer, andere Formen der Installierbarkeit ohne viel vorheriges Fachwissen?
* Gibt es ausreichend Tutorials für das Erlernen der Software? Hier sollte überprüft werden, ob die Tutorials auf unterschiedliches Vorwissen eingehen und gegebenenfalls auch kenntlich machen, welches Grundwissen, welche Erfahrungen unabdingbar sind. Ein weiterer Aspekt bei den Anleitungen, Tutorials und FAQs ist die Frage der Sprachen.
* Sind die Entwickler der Software aktiv und gut erreichbar? Wird die Software regelmäßig mit Updates versorgt?
* Wird die Software von einer Community getragen? Die Zahl der aktiven Nutzer eines Softwarewerkzeugs ist entscheidend dafür, ob man im Falle von Problemen schnell Hilfe googeln kann. Ist das Werkzeug das Erzeugnis eines einzigen Labors und wird von einer Hand voll eingeschworener Kollegen genutzt, oder handelt es sich um eine global etablierte Software mit Nutzerforum, Mailingliste und ganzen Büchern zur Nutzung in bestimmten Kontexten? Selbst wenn ein Werkzeug nur eine kleine Community besitzt kann dieser Mangel doch bis zu einem gewissen Grad von aktiven und leicht erreichbaren Entwicklern ausgeglichen werden, die bereit sind konkrete Fragen schnell und unkompliziert zu beantworten.
* Gibt es bereits eine speziell archäologische Community für diese Software? (SIG, ...).
* Haben ArchäologInnen bereits Best Practices für diese Software formuliert?
* Gibt es Archäologie-relevante erfolgreiche Projekte/Anwendungen, die von dieser Software bereits unterstützt wurden?

> [MT] folgendes wurde aus dem FAIR-Teil hier her verschoben; muss dann noch eingearbeitet Werden

Unter Nutzbarkeit wird oftmals allein UX Design verstanden, was Fragen der Gestaltung und Bedienbarkeit grafischer Oberflächen von Programmen (GUI) und Webseiten beinhaltet. Hier geht es dann um die Benutzbarkeit von Webanwendungen mit verschiedenen Endgeräten (Responsivität), die Strukturierung von Informationen über die Menüführung hinweg, die Verständlichkeit von Texten und auch die Barrierefreiheit (Farbkontraste, Screenreader u.ä.).

Usability umfasst aber noch mehr und schließt alle Aspekte ein, die eine fehlerfreie und effiziente Nutzung durch die Forscherin, den Forscher ermöglichen. Für Forschungssoftware ist es z.B. besonders wichtig, dass die Eingabe von Daten sich an der Eingabepraxis orientiert; wenn etwa die händische Eingabe von Werten sehr typisch ist, dann ist es Aufgabe einer guten Benutzbarkeit, diesen Vorgang mit vorgegebenen Feldformaten, automatischem Speichern, gut sichtbaren Feldern oder ähnlichem zu unterstützen. Ebenso muss Software die üblicherweise von Teams genutzt wird, in denen verschiedene Kompetenzen vertreten sind, ein Rechtemanagement vorsehen, das die unterschiedlichen Verantwortlichkeiten abbilden kann. Forschungssoftware wird nicht im leeren Raum genutzt, sondern trifft auf Erwartungen und Gewohnheiten der Nutzer\*innen, sowohl was ihre Bedienung betrifft, als auch die ergänzenden Angebote zur Unterstützung, wie Tutorials FAQs und ähnliches. Software, die für hochspezielle Fragestellungen verwendet wird, die auf einer Reihe vorhergehender Prozessschritte aufbaut, richtet sich an einen anderen Nutzerkreis, als Software, die Basisfunktionen erfüllt. Weil Forscher\*innen am besten beurteilen können, ob ihre Bedarfe und Gewohnheiten gut adressiert sind und die Forschungssoftware ihnen ein gutes Arbeiten erlaubt, gehört eine Beurteilung dieser Aspekte in die Rezension.
Ableiten lassen sich Kriterien, auf die sich die Nutzungserfahrung abbilden lässt aus der Forschung und den Referenz-Standards zur Usability. Zu nennen ist unter anderem der ISO/IEC 9126 Standard und spezifisch für Webanwendungen bilden die Empfehlungen und Standards des W3C [@noauthor_w3c_nodate](#noauthor_w3c_nodate).  

### Technik

Weiter oben haben wir die handwerkliche Qualität von Software aus der Anwender-Perspektive betrachtet. Hier geht es nun um Fragen, die direkt den Programmcode betreffen. Eine Beurteilung derselben erfordert also, den Programmcode herunterzuladen und in Stichproben durchzusehen. Das ist bei proprietärer Software meist nicht möglich.

#### Qualität der Implementierung
* Entspricht die Implementierung dem Stand der Technik?
* Ist die Implementierung performant? Für Webapplikationen und Plugins ist zu überprüfen, ob sie responsiv sind und über die verschiedenen Browser hinweg performant sind.
* Wie robust ist die Software gegenüber äußeren Einflüssen? Wie geht die Software mit Abstürzen/Stromausfall usw. um? Wird die Arbeit regelmäßig zwischengespeichert?

#### Dokumentation und Tests
* Ist eine Quellcodedokumentation vorhanden und ggf. eine HTML Variante davon verfügbar?
* Ist der Buildprozess dokumentiert und ggf. mittels Buildingscripts automatisiert?
* Gibt es eine Entwicklerdokumentation, sodass die Software leichter verstanden werden und ggf. erweitert werden kann?
* Ist die Dokumentation aktuell, wird gepflegt und deckt alle Funktionen des Programms ab?
* Hat der Quellcode Tests, die die Kernfunktionen des Programms testen und diese für andere Entwickler aufzeigen?
* Sind verwendete Algorithmen dokumentiert und hinreichend wissenschaftlich belegt?

#### Sicherheit
* Ist die Anwendung auf Sicherheitsanforderungen getestet worden? (Penetrationtests usw.), also ist sie leicht hackbar oder nicht?
* Setzt die Anwendung Standards zur IT Sicherheit welche von Behörden oder internationalen Organisationen empfohlen werden um? Beispiel [OWASP](https://de.wikipedia.org/wiki/Open_Web_Application_Security_Project)
* Hat die Anwendung Abhängigkeiten zu Softwarekomponenten welche bekannte Sicherheitslücken aufweisen und nicht mehr gepflegt werden? Hält dieser Zustand auf absehbare Zeit an?

### Rechtliche Fragen

Software muss sich wie alle wissenschaftlichen Werkzeuge in einen rechtlichen Rahmen einordnen. Dabei sind die Aspekte Lizenzierung und Datenschutz von besonderer Bedeutung.

#### Lizenzierung
* Ist die Software frei/Open Source?
* Sind die Ressourcen, die mit der Software mitgeliefert werden unter einer freien Datenlizenz verfügbar? (beachte: Copyright und Copyleft, Problem von Creative Commons `non commercial`)
* Erlaubt die Software nur die Erstellung von Daten, die unter einer gewissen Lizenz zur Verfügung gestellt werden können?
* Behält sich die Software Rechte an den von ihr erstellten Daten vor?

#### Datenschutz, Privacy, Datensparsamkeit
* Beachtet die Software die lokalen Gesetze in dem Land in dem sie eingesetzt werden soll? (Datenschutz, Kartendarstellungen etc.)?
* Welche Daten speichert die Anwendung zu welchem Zweck wie lange? Dienen diese Daten der Forschung bzw. helfen sie die Software zu verbessern?
* Ist die Software ohne Login anonym bedienbar?
* Benötigt die Software eine Internetverbindung und werden personenbezogene Daten an Dritte übertragen?


## Anmerkungen

<a name="myfootnote1">1</a>: Aufgeworfen und anschließend im Plenum des 9. Workshops der deutschen Sektion der CAA 2019 in Wilhelmshaven wurde die Frage nach den Inhalten einer Rezension von Software und Anwendungen für die Archäologie von Sophie Charlotte Schmidt, Kai-Christian Bruhn und Siegmund Freud. Anlässlich der Einrichtung der neuen Rubrik für solche Besprechungen in der vorliegenden Reihe haben wir das Thema aufgegriffen und möchten mit der vorliegenden Handreichung einen Beitrag zur Weiterentwicklung dieses wichtigen Themas leisten. Die Handreichung kann auch zur Orientierung bei Entscheidungen zum Einsatz einer Software in der eigenen Forschung dienen.


## Bibliographie
