# Thermografische Gebouwanalyse

## Inleiding

Dit applicatieprofiel dient als weergave van het stapsgewijs proces rond het maken, verwerken en interpreteren van thermografische scans van gebouwen.

Thermografische Gebouwanalyse zich op het gebruik van een voertuig uitgerust met een thermografische camera, de Thermocar, om gebouwgevels te scannen en gebieden met energieverlies te identificeren. Deze gegevens worden vervolgens verwerkt om huiseigenaren gericht renovatieadvies te geven. De huidige handmatige gegevensverwerking is echter tijdrovend en zorgt voor lange wachttijden voor bewoners.

De interpretatie kan zowel manueel gebeuren, maar dankzij het gebruik van AI kan dit ook geautomatiseerd verlopen. Dit traject, Thermografische Gebouwanalyse, had dan ook bijzondere aandacht voor deze automatisatie. Dit traject werd opgezet door de [West-Vlaamse Intercommunale (WVI)](https://www.wvi.be/) en ondersteund door [Stad Brugge](https://www.brugge.be/).

Om de eigenlijke Observatie en bijbehorende informatie rond de Observatieprocedure, het ObserveerbaarKenmerk, de Observatieverzameling en de Sensor te capteren, werden deze klassen overgenomen uit het internationaal erkende [Semantic Sensor Network Ontology (SSN)](https://www.w3.org/TR/vocab-ssn/). Een Observatie wordt steeds uitgevoerd met een Sensor, dewelke nog verschillende subklasses heeft. De subklasses, die relevant zijn voor het maken van thermografische scans, en dus nieuw werden gedefinieerd voor dit traject, zijn: Camera, GPS, en Opstelling. Daarnaast werd, om informatie te capteren rond het gebruikte AI model voor intepretatie van de beelden, ook de klasse MachineLearning Model overgenomen uit [MLDCAT-AP](https://semiceu.github.io/MLDCAT-AP/releases/2.0.0/). Ook deze klasse wordt in het model als subklasse van Sensor gezien

Het is belangrijk om te begrijpen dat de klasse Observatie een representatie is van elke stap in het proces, gaande van de effectieve Meting, tot Classificatie, tot GeometrieObservatie en de eigenlijke Interpretatie. De eerste drie subklasses zijn overgenomen uit [OSLO Observaties en Metingen](https://data.vlaanderen.be/doc/applicatieprofiel/observaties-en-metingen/), terwijl Interpretatie nieuw gedefinieerd werd in dit traject.

De Observatie zelf werd op het hoogst mogelijke niveau gemodelleerd, door het gebruik van de klasse Any. Deze klasse is zelf overkoepelend voor de subklasse Domeinobject, wat erop wijst dat de oberservatie in dit model steeds op een vast, niet-bewegende object gebeurt. Dit Domeinobject is namelijk ook overkoepelend voor de nieuwe gedefinieerde klassen Video en Foto, alsook de herbruikte klassen Gebouw, Gebouweenheid, BIM_Gebouw en BIM_Element. Deze werden respectievelijk overgenomen uit [OSLO Gebouw](https://data.vlaanderen.be/ns/gebouw/) en [IFC](https://www.buildingsmart.org/standards/bsi-standards/industry-foundation-classes/).

Tenslotte zijn er ook nog enkele klassen aan het model toegevoegd, die nog meer informatie kunnen bieden omtrent de gebruikte Toestel, Systeem, bijbehorend Deployment en het Platform waarop dit Systeem gehost wordt. Deze klassen zijn allen afkomstig van [Semantic Sensor Network Ontology (SSN)](https://www.w3.org/TR/vocab-ssn/), alsook de [Smart Applications REFerence ontology (SAREF)](https://saref.etsi.org/core/v4.1.1/).

Dankzij deze semantische standaard wordt de uitwisseling tussen o.a. gemeentelijke en geografische systemen bevordert en de doorzoekbaarheid en vindbaarheid vergemakkelijkt.

## Verslagen en presentaties

De verslagen en presentaties van dit traject kan je terugvinden op het [Standaardenregister](https://data.vlaanderen.be/standaarden/applicatieprofiel-thermografische-gebouwanalyse).

## In deze repository

EAP-files met de UML-diagrammen.\
Configuratie en bestanden voor het publiceren van de specs in de folders config, site-skeleton en templates.\
Een [changelog](./CHANGELOG) met wijzigingen tov vorige versies.\
Diverse resources:
- Een overzicht van de [use cases]()
- Een overzicht van gebruikte [bronnen]() (standaarden, implementaties, regelgeving).
- Het [modelleringsrapport](https://github.com/Informatievlaanderen/OSLOthema-thermAI/blob/main/resources/ModelleerrapportThermAI.pdf).
- Een map met [datavoorbeelden](hhttps://github.com/Informatievlaanderen/OSLOthema-thermAI/tree/main/resources/Datavoorbeelden).

## Issues

Via de tab [issues](https://github.com/Informatievlaanderen/OSLOthema-thermAI/issues) kan je opmerkingen en feedback over het model geven.

## Publicaties

Volgende specificaties worden met de volgende status voorgelegd op WG datastandaarden van 22 mei 2025.

| Naam|Status|Uitgiftedatum|AP|VOC|
| --- |--- |---|---|---|
|Thermografische gebouwanalyse|OntwerpStandaard|20250522|[Link](https://data.vlaanderen.be/doc/applicatieprofiel/thermografische-gebouwanalyse/)|NVT|

