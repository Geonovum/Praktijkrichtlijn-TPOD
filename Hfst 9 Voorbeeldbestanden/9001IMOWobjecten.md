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



