####Voorbeeldbestanden

Een voorbeeldbestand is een technisch voorbeeld hoe een omgevingsdocument eruit kan zien en welke onderdelen
deze kan bevatten. Het zijn technische voorbeelden en niet perse in logische tekst.

Elk voorbeeld bestand bevat:

-   Het *besluit*: Deze heeft een AKN identifier en heet AKN_NL_bill_<afkorting bevoegd gezag><cbscode bevoegd gezag>-<nummer>.xml

-   Twee *manifesten*: Dit zijn manifest.xml (voor LVBB) en owmanifest.xml (voor OZON/DSO-LV). Dit is de pakbon van
    alle bestanden die nodig zijn voor publicatie op de LVBB respectievelijk DSO-LV. 

-   Een *opdracht*: Deze heet opdracht.xml. Hierin staan het versienummer van de standaard en een publicatieopdracht.

-   Een of meerdere *GML*-bestanden: Deze heten <gebiedsnaam of nummer>.gml. Hierin zijn de locaties met bijbehorende geometrie te vinden.

-   Minstens een *Geografische informatieobject*: Deze heeft een naam die opgebouwd is uit GIO<gebiedsnaam of nummering>.xml. Dit bestand bevat
    STOPdata en de verwijzing naar een of meerdere gml bestanden. Er kunnen meerdere GIO's voorkomen om verschillende gebieden aan te duiden.

-   Alle *owObjecten*: Dit zijn losse bestanden in xml-formaat per owObject, bijvoorbeeld: owActiviteiten, owGebiedsaanwijzingen, owLocaties, 
    owPons, etc



####IMOW objecten

**Regeltekst**

In het regeltekst-bestand leg je de koppeling tussen de gegevens vanuit het IMOP en het IMOW. Dit gebeurt middels het OwObject van Regeltekst. 
Deze Regeltekst bevat twee attributen die verwijzen naar het IMOP, dit zijn wId en WorkIDRegeling.
-   wId verwijst naar het ID van het artikel of lid uit IMOP.
-   WorkIDRegeling verwijst naar het ID van de regeling uit IMOP.

Regeltekst heeft zelf ook nog een identificatie, hier wordt naar verwezen vanuit OwObjecten. In het document met Regeltekst dien je ook 
Juridische Regels te definiëren. Een juridische regel maakt het mogelijk om te duiden welke OwObjecten worden aangemerkt in een bepaald 
artikel of lid.
Juridische Regel is een abstract objecttype dat drie subtypen heeft, namelijk: RegelVoorIedereen, Instructieregel en Omgevingswaarderegel.
De Juridische regels hebben een identificatie en een attribuut genaamd: ‘artikelOfLid’, welke verwijst naar de OW-Regeltekst. 
Vul hierin dezelfde waarde van identificatie in als de waarde die is opgenomen in de OW-Regeltekst.identificatie.

Daarbij kennen OwObjecten ook onderlinge relaties. Zo heeft een Juridische regel een relatie naar o.a. een Activiteit, Omgevingsnorm, 
Gebiedsaanwijzing en andere. De XSD’s kennen hiervoor een Ref element, zoals ActiviteitenRef. Vul hierin de identificatie in van het 
gerelateerde objecttype, oftewel de waarde die staat in het element identificatie van het desbetreffende object.

**OW-annotaties**

Naast Regeltekst zijn er meerdere OwObjecten die meegeleverd kunnen worden. Zo heeft een Activiteit een relatie naar een Locatie. 
De XSD’s kennen hiervoor een Referentieelement, zoals LocatieRef. Vul hierin de identificatie in van het gerelateerde objecttype, dit is de
waarde die staat in het element identificatie van het desbetreffende object.
Het is de bedoeling dat de identificaties van OW-objecten in de OW-bestanden geschikt moeten zijn
voor het bevoegd gezag (BG) zelf en voor gebruik/afname vanuit de landelijke voorziening digitaal
stelsel Omgevingswet (DSO-LV) door het DSO, de BG en derden.


**Identificatie OW-object**

De identificatie van een OW-object, zoals een Locatie, krijgt daarom bij BG een lokale identificatie die bepaald wordt door BG zelf. 
Deze lokale identificatie komt vervolgens in alle ketens herkenbaar beschikbaar en moet daarom globaal uniek zijn, of gemaakt (kunnen) worden, zodat deze geschikt is
voor gebruik in de LVBB en DSO-LV en afnemers daarvan.
Onderstaande beschrijft de specificatie hiervoor. De lokale identificatie vormt de basis voor de keten van BG naar DSO en weer terug naar BG of derden.

-   Bij uitwisseling van informatie in ketens met andere partijen, dan wordt deze lokale identificatie globaal uniek gemaakt, via vaste 
    afspraken (zie IMOW).

-   Keten van plan tot publicatie, opname in OP bestanden: zie OP specificatie.

-   Keten van plan tot publicatie, opname in OW bestanden: zie hieronder.

Als er sprake is van informatie die én in OW-bestanden zit én in OP-bestanden zit, dan is de lokale identificatie het verbindende gegeven.



####OW-manifest

De OW bestanden zijn opgesomd in het ow specifieke manifest. Hierin plaats je de versie van de regeling waar de aanlevering bij hoort. 
Vervolgens specificeer je in dit bestand de OW-specifieke annotaties die je meelevert. Hierdoor staat per OW-bestand alleen dezelfde soort 
objecten gedefinieerd.



####GML-bestanden

De gml specificaties volgen de regels van de standaard Basisgeometrie:
https://docs.geostandaarden.nl/nen3610/basisgeometrie/

Het bijbehorende GML applicatieschema Basisgeometrie.xsd is gepubliceerd op:
https://register.geostandaarden.nl/gmlapplicatieschema/basisgeometrie/

De inhoud van de genoemde standaard Basisgeometrie en het schema zijn ook opgenomen in IMOW.



