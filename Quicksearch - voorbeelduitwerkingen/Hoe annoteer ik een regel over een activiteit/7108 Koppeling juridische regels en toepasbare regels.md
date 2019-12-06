#### Koppeling juridische regels en toepasbare regels via IMOW activiteit

Bovenstaande IMOW-attributen van het object activiteit borgen de koppeling
tussen juridische regels en toepasbare regels. Onderstaande figuur toont de
koppeling tussen juridische regels en toepasbare regels voor wat betreft de
functionele structuur, waar de attributen identificatie, naam en bovenliggende
activiteit een rol bij spelen. De locatieaanduiding is niet toegelicht, omdat
deze in de opsomming hierboven al is uitgewerkt.

![](media/7108JRTRactiviteitFS.png)

*Koppeling IMOW-object activiteit en functionele structuur*

De toelichting op bovenstaande figuur volgt in onderstaande opsomming:

>   1: Vanuit de wet / AMvB ( / MR) komen er Rijks-activiteiten terecht in de
>   Functionele Structuur. Deze Rijksactiviteiten komen als IMOW-activiteiten
>   via een omgevingsdocument (via LVBB-\>OZON) terecht in de functionele
>   structuur.  
>   In bovenstaande figuur is de activiteit “Activiteiten met gevolgen voor de
>   fysieke leefomgeving” het hoogste niveau (hiërarchisch), die via de
>   wet in de Functionele Structuur terecht komt. Onder deze activiteit valt 
>   o.a. de activiteit “Omgevingsplanactiviteit” die door het IMOW-deel van de wet / 
>   AMvB in de Functionele Structuur terecht komt.  
>   Ook het gegeven dat “Activiteiten met gevolgen voor de fysieke leefomgeving”
>   de bovenliggende activiteit is van “Omgevingsplanactiviteit” komt via het
>   IMOW-deel van de wet / AMvB terecht in de functionele structuur. Bij het maken van
>   de activiteit "omgevingsplanactiviteit", wordt in het attribuut bovenliggende activiteit 
>   aangegeven dat dit "Activiteiten met gevolgen voor de fysieke leefomgeving" is.

>   2: Voor elk nieuw omgevingsdocument dat een IMOW-deel bevat met daarin
>   activiteit-objecten, geldt dat nieuwe activiteiten gerelateerd moeten worden
>   aan bestaande activiteiten. 
>   Bijvoorbeeld: Het omgevingsplan bevat een object
>   Activiteit “Bouwactiviteit” die tot dan toe niet voorkomt in de functionele
>   structuur. IMOW stelt voor “Bouwactiviteit” een identificatie op
>   gnm0037.Activiteit.2019000241. Deze *nieuwe* activiteit “Bouwactiviteit”
>   moet in het IMOW-deel van het omgevingsplan gerelateerd worden aan de
>   *bestaande* activiteit “Omgevingsplanactiviteit”, zodanig dat de
>   Omgevingsplanactiviteit de bovenliggende activiteit is van Bouwactiviteit.
>   Het relateren aan de activiteit “Omgevingsplanactiviteit” verloopt via de
>   identificatie hiervan (in bovenstaand figuur mn002.Activiteit.FunctioneleStructuur0010).

>   3: Op het moment dat het IMOW-deel van het omgevingsplan in OZON terecht
>   komt, wordt vervolgens de Bouwactiviteit(en) in de functionele structuur
>   ondergebracht bij de bovenliggende activiteit waar het volgens de
>   aanlevering bij hoort.

>   4, 5: Het kan zijn dat in een omgevingsdocument een nieuwe activiteit die
>   het vastlegt, *zelf* een bovenliggende activiteit is van andere nieuwe
>   activiteiten die het omgevingsbesluit vastlegt. In bovenstaand voorbeeld
>   vormt Bouwactiviteit de bovenliggende activiteit van Bijbehorend bouwwerk
>   bouwen en van Dakkapel bouwen. Alle drie de activiteiten zijn nieuwe
>   activiteiten die zijn vastgelegd in het omgevingsdocument. Om ervoor te
>   zorgen dat Bouwactiviteit de bovenliggende activiteit wordt van de andere
>   twee activiteiten, dienen deze beide activiteiten een bovenliggende
>   activiteit-relatie aan te brengen naar de identificatie van Bouwactiviteit
>   (in bovenstaande figuur gm0037.Activiteit.201900024). Daarnaast krijgen
>   Bijbehorend bouwwerk bouwen en Dakkapel bouwen hun eigen identificatie
>   (resp. gm0037.Activiteit.2019000243 en gm0037.Activiteit.2019000242).

>   6,7: Zodra het omgevingsdocument en het IMOW-deel ervan in OZON terecht
>   komt, worden alle IMOW-activiteit objecten ondergebracht in de functionele
>   structuur. Dit wordt mogelijk gemaakt door de verplichting in IMOW op de
>   bovenliggende activiteit relatie. Uiteindelijk moet iedere activiteit gekoppeld
>   zijn aan een activiteit uit de functionele structuur, hetzij direct of indirect (middels
>   de bovenliggende activiteiten). Als in een omgevingsdocument nieuwe activiteiten 
>   vastgelegd worden die onderling elkaars bovenliggende activiteiten vormen, dient de 
>   bovenste activiteit verplicht een bovenliggende activiteit-relatie te krijgen met een 
>   activiteit die reeds voorkomt in de functionele structuur.

Het IMOW-attribuut activiteitregelkwalificatie, dat een nadere kwalificatie van
een juridische regel over een activiteit geeft (bijvoorbeeld: vergunningplicht,
meldingsplicht of verbod) speelt geen rol in de koppeling van juridische regels
en toepasbare regels.