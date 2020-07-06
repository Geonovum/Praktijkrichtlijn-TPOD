####Uitleg voorbeeldbestanden

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



