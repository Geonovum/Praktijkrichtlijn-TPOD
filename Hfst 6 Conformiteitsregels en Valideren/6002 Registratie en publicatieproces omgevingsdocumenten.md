####Registratie en publicatie van een omgevingsdocument

Dit proces betreft de primaire transacties die plaatsvinden bij een instellingsbesluit of wijzigingsbesluit over 
een regeling die een omgevingsdocument betreft. Het betreft het geheel aan gegevens, dus zowel IMOP-deel als IMOW-deel. 
Op conceptueel niveau verloopt het proces als volgt:
 
![](media/6002Validatieproces_registratie_publicatie_omgevingsdocument.png)

*Validatieproces bij registratie en publicatie omgevingswetbesluit*  
 
In bovenstaande figuur wordt het begrip ‘besluit’ gehanteerd dat in brede context moet worden geplaatst. Het betreft 
in elk geval alle initiële besluiten, wijzigingsbesluiten, niet-consoliderende besluiten, rectificaties en directe mutaties.  
Bij alle stappen in dit proces kan uitval voorkomen, zowel in de (ongenummerde) transmissie als in de (genummerde) inhoudelijke
verwerking. De validatieregels in de bijgevoegde validatiematrix gaan alleen in op de laatste categorie: op welke stap in het 
proces wordt een validatieregel uitgevoerd en welk gedrag is er nodig bij afkeur van gegevens. 
 
Korte toelichting per stap:
1. Validatie van de opdracht door LVBB bronhouderkoppelvlak: Als een bevoegd gezag een besluit of mutatie verstuurt aan het LVBB 
   Bronhouderkoppelvlak, dan vinden in het bronhouderkoppelvlak technische validaties plaats op het niveau van het berichtenverkeer 
   die zich richten op de vraag of de ontvangen opdracht te begrijpen is (zoals: is het een valide ZIP, zijn alle bestanden aanwezig, 
   zijn er geen onverwachte bestanden?). 
2. Validatie van STOP-besluit door LVBB Publicatiecomponent: Een juridisch besluit met betrekking tot een omgevingsdocument wordt 
   gevalideerd door het LVBB Publicatiecomponent. 
3. Validatie van geometrie door Kadaster: De geometrie van het besluit wordt gevalideerd, zoals bijvoorbeeld vastgelegd in een 
   geo-informatieobject (GIO). 
4. Validatie van domeingegevens door DSO-LV OZON: De OZON-component van DSO-LV valideert de bij het besluit aangeleverde domeingegevens.  
5. Evaluatie door LVBB Bronhouderkoppelvlak: Door het LVBB Bronhouderkoppelvlak wordt bepaald of een aangeleverd besluit voldoet aan 
   alle eisen voor LVBB Publicatiecomponent en DSO-LV. Hier wordt een evaluatie gedaan van resultaten bij de stappen 2 t/m 4. 
6. Publicatie van besluit door LVBB Publicatiecomponent: Het besluit wordt middels publicatie door LVBB Publicatiecomponent officieel 
   bekendgemaakt. 
7. Consolidatie van besluit naar regelingversie door LVBB Publicatiecomponent: Het besluit wordt geconsolideerd in de huidige regeling, 
   zodat een nieuwe regelingversie ontstaat. Bij ontwerp-besluiten wordt een ‘toekomstige regelingversie’ gemaakt, dit is geen feitelijke 
   consolidatie van regelgeving. Bij nietconsoliderende besluiten, rectificaties en directe mutaties heeft deze stap wellicht een iets 
   andere betekenis dan een echte consolidatie. 
8. Objectvorming bij DSO-LV OZON: Op basis van de ontstane regelingversie en domeingegevens worden informatieobjecten gemaakt voor de
   objectgerichte ontsluiting binnen DSO-LV. 
 
