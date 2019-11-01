#### Relatie met Functionele structuur en toepasbare regels

De koppeling tussen juridische regels en toepasbare regels begint bij het object
activiteit binnen IMOW. Merendeel van de attributen van de activiteit worden
gebruikt door de toepasbare regel. De activiteitgroep vormt hier een
uitzondering op, deze is niet opgenomen in onderstaande opsomming:

-   *Identificatie en naam*: de naam en identificatie worden opgeslagen in het
    DSO, zowel in OZON als in de functionele structuur binnen het Register
    Toepasbare Regels, die gevoed wordt door het IMOW-deel van
    omgevingsdocumenten.

-   *locatieaanduiding*: toepasbare regels halen hun locatie uit de
    locatieaanduidingen die de activiteit in IMOW aanduid.

-   *bovenliggende activiteit*: de verwijzing van een specifieke activiteit naar
    een andere activiteit, die in de taxonomie van activiteiten (de functionele
    structuur), taxonomisch meer classificerend of inhoudelijk generieker is dan
    de activiteit die wordt geannoteerd. Zo kan het ‘houden van kippen’ vallen
    onder ‘houden van dieren’, of het ‘opslaan van brandstoffen’ onder
    ‘milieubelastende activiteiten’. De bovenliggende activiteit bepaalt waar in
    de functionele structuur de Activiteit zal worden toegevoegd.

-   *gerelateerde activiteit*: Een secundaire (d.w.z. niet verplicht)
    aanknopingspunt tussen juridische regels en toepasbare regels vormen
    relaties tussen activiteiten die geen hiërarchie / taxonomie aanduiden, maar
    die aanduiden dat activiteiten op enigerlei andere wijze contextueel
    relevant met elkaar zijn.

**Koppeling juridische regels en toepasbare regels via IMOW activiteit**

Bovenstaande IMOW attributen van het object activiteit borgen de koppeling
tussen juridische regels en toepasbare regels. Onderstaande figuur toont de
koppeling tussen juridische regels en toepasbare regels voor wat betreft de
functionele structuur, waar de attributen identificatie, naam en bovenliggende
activiteit een rol bij spelen. De locatieaanduiding is niet toegelicht, omdat
deze in de opsomming hierboven al is uitgewerkt.

![](media/7133JRTRactiviteitFS.png)

*Koppeling juridische regels en toepasbare regels via IMOW activiteit en
Functionele Structuur*

De toelichting op bovenstaande figuur volgt in onderstaande opsomming:

>   1: Vanuit de wet / AMvB ( / MR) komen er Rijks-activiteiten terecht in de
>   Functionele Structuur. Deze Rijksactiviteiten komen als IMOW activiteiten
>   via een omgevingsdocument (via LVBB-\>Ozon) terecht in de Functionele
>   Structuur.  
>   In bovenstaande figuur is de activiteit “Activiteiten met gevolgen voor de
>   fysieke leefomgeving” het topniveau van de Functionele Structuur, welke via
>   de wet in de Functionele Structuur terecht komt.  
>   Onder deze activiteit valt o.a. de activiteit “Omgevingsplanactiviteit”
>   welke door het IMOW-deel van de wet / AMvB in de Functionele Structuur
>   terecht komt.  
>   Ook het gegeven dat “Activiteiten met gevolgen voor de fysieke leefomgeving”
>   de bovenliggende activiteit is van “Omgevingsplanactiviteit” komt via het
>   IMOW-deel van de wet / AMvB terecht in de Functionele Structuur. Hiervoor
>   wordt het attribuut *bovenliggende activiteit* van het IMOW object
>   activiteit gebruikt.

>   2: Voor elk nieuw omgevingsdocument dat een IMOW-deel bevat met daarin
>   activiteit-objecten, geldt dat nieuwe activiteiten gerelateerd moeten worden
>   aan bestaande activiteiten.
>   Bijvoorbeeld: Het omgevingsplan bevat een object Activiteit
>   “Bouwactiviteiten” die tot dan toe niet voorkomt in de Functionele
>   Structuur. IMOW stelt voor “Bouwactiviteiten” een identificatie op
>   gnm0037.Activiteit.2019000241.
>   Deze *nieuwe* activiteit “Bouwactiviteiten” moet in het IMOW-deel van het
>   omgevingsplan, gerelateerd worden aan de *bestaande* activiteit
>   “Omgevingsplanactiviteit”, zodanig dat de Omgevingsplanactiviteit de
>   bovenliggende activiteit is van Bouwactiviteiten.
>   Het relateren aan de activiteit “Omgevingsplanactiviteit” verloopt via de
>   identificatie hiervan (in bovenstaand figuur
>   mn002.Activiteit.FunctioneleStructuur0010).

>   3: Op het moment dat het IMOW-deel van het omgevingsplan in OZON terecht
>   komt, wordt vervolgens de Bouwactiviteit(en) in de Functionele Structuur
>   ondergebracht bij de bovenliggende activiteit waar het volgens IMOW bij
>   hoort.

>   4, 5: Het kan zijn dat in een omgevingsbesluit, een nieuwe activiteit die
>   het vastlegt, *zelf* een bovenliggende activiteit is van andere nieuwe
>   activiteiten die het omgevingsbesluit vastlegt. In bovenstaand voorbeeld
>   vormt Bouwactiviteiten de bovenliggende activiteit van Bijbehorend bouwwerk
>   bouwen en van Dakkapel bouwen. Alle drie de activiteiten zijn nieuwe
>   activiteiten vastgelegd in het omgevingsdocument. Om ervoor te zorgen dat
>   Bouwactiviteiten de bovenliggende activiteit wordt van de andere twee
>   activiteiten, dienen deze beide activiteiten een *bovenliggende
>   activiteit*-relatie aan te brengen naar de identificatie van
>   Bouwactiviteiten (in bovenstaande figuur gm0037.Activiteit.201900024).
>   Daarnaast krijgen Bijbehorend bouwwerk bouwen en Dakkapel hun eigen
>   identificatie (resp. gm0037.Activiteit.2019000243 en
>   gm0037.Activiteit.2019000242).

>   6,7: Zodra het omgevingsdocument en het IMOW-deel ervan in OZON terecht
>   komt, worden alle IMOW-activiteit objecten ondergebracht in de Functionele
>   Structuur.
>   Dit wordt mogelijk gemaakt door de verplichting in IMOW op de *bovenliggende
>   activiteit* relatie:
>   -   Als een juridische regel in een omgevingsbesluit slechts één nieuwe IMOW
>       activiteit object bevat, heeft deze verplicht een *bovenliggende
>       activiteit*-relatie met een activiteit die reeds voorkomt in de Functionele
>       Structuur.
> -     Als in een omgevingsbesluit er nieuwe activiteiten vastgelegd worden die
>       onderling elkaars *bovenliggende activiteiten* vormen, dient de bovenste
>       activiteit verplicht een *bovenliggende activiteit*-relatie te krijgen met
>       een activiteit die reeds voorkomt in de Functionele Structuur.

Het IMOW-attribuut Regelkwalificatie, dat aangeeft welke plicht bij een activiteit wordt aangegeven 
(bijvoorbeeld: vergunnings-, meldingsplicht of verbod) speelt geen rol in de koppeling van 
juridische regels en toepasbare regels.