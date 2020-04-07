#### Classificatie van validatie- en conformiteitsregels nader bekeken

Op basis van het eerder beschreven validatieproces wordt een vaste classificatie 
van validatieregels gehanteerd, als informatie over of documentatie van de validatieregel. 
Het geharmoniseerde overzicht met validatie-en conformiteitsregels zijn opgenomen in eenseparaat 
aangeleverde validatiematrix. De classificaties die zijn aangegeven met (*) worden teruggekoppeld 
aan het systeem van bevoegd gezag bij het verzenden van de resultaatmeldingen aan het eind van 
het proces. 
 
**ID (*)** 
Iedere validatieregel heeft een uniek identificatienummer. Deze nummering wordt toegekend door 
de beheerders van de respectievelijke validatieregels. De opbouw van dit ID is vier letters en 
vier cijfers. Toekenning van ID’s wordt in overleg gedaan door de partij die ook de validatieregel 
zelf beheert. 
 
**Beschrijving (*)** 
Iedere validatieregel wordt in een beknopte, leesbare tekst beschreven. In de documentatie is een uitgebreidere 
beschrijving mogelijk waar dit nodig is. 
 
**Type Er zijn drie soorten validatieregels:**
- Validatie: Het bestand zelf wordt op validiteit gecontroleerd; 
- Verificatie: Het bestand wordt vergeleken en getoetst met reeds 
  in het systeem aanwezige informatie en/of meegeleverde informatie 
  in een ander bestand. 
- Richtlijn: Er wordt gecontroleerd of een bepaald aspect van de informatie 
  conform die hiervoor geldende standaard is ingezet.  
 
**Bron (*)** 
Iedere validatieregel heeft een referentie, bron, grondslag of herkomst. 
Geldige bronnen zijn op dit moment: 
- PKI-Overheid 
- Digikoppeling 
- STOP  
- TPOD  
- IMOW  
- GML 3.2.1 SF2 
- ETRS89 - RD 
- DSO-LV 
- Werkafspraak *)   
  *)Met een perfecte standaard is dit een lege verzameling. 
  Het komt echter voor dat een standaard ongewenste vrijheidsgraden of fouten 
  heeft die tot implementatieproblemen leiden. In dat geval kan een tijdelijke 
  werkafspraak worden gemaakt met het werkveld, vooruitlopend op de aanpassing 
  van de standaard. 
 
**Subject** 
Op welk gegeven of bestand wordt de validatieregel uitgevoerd. 
Geldige waarden:   
- Leveringsverzoek 
- Opdracht 
- STOP bestand 
- GML bestand 
- IMOW bestand 
- Besluit 
- Officiële Publicatie 
- Regelingversie 
- Toestand 
 
**Ernst (*)** 
Iedere validatieregel is geclassificeerd met een foutcode. 
Geldige waarden: 
- Blokkerend: als niet aan deze regel wordt voldaan, dan treedt uitval op conform 
  bovenstaande beschrijvingen; 
- Waarschuwing: als niet aan deze regel wordt voldaan dan treedt er geen uitval op, 
  maar wordt er een waarschuwing 
  gegenereerd door het validerende systeem; 
- Richtlijn: als niet aan deze regel wordt voldaan, dan wordt er een inhoudelijke fout 
  gemaakt. Echter, deze validatieregel wordt nergens technisch afgedwongen en leidt niet 
  tot uitval; 
- Info: De validatieregel leidt tot neutrale informatieve meldingen. 
 
**Melding aan** 
Iedere validatieregel leidt tot een mogelijke melding. Dit is de beoogde ontvanger van deze melding. 
Geldige waarden: 
- BG: systeem van bevoegd gezag dat de gegevens heeft aangeleverd. 
- Intern: het systeem dat de melding heeft geconstateerd. De meldingen van deze validatieregels 
  gaan dus niet terug in de resultaatmeldingen naar het systeem van bevoegd gezag. 
 
**Validator** 
Dit veld geeft aan welke component de validatie uitvoert. 
Geldige waarden: 
- LVBB-BHK: het bronhouderkoppelvlak van de LVBB 
- LVBB-PUB: het publicatiecomponent van de LVBB 
- DSOLV-OZON: het OZON-component van DSO-LV 
- Kadaster: generieke geo-validatiecomponent van het Kadaster 
 
**Regelingtype** 
Er zijn validatieregels die niet voor alle typen regelingen of besluiten van regelingen van toepassing zijn. 
Geldige waarden zijn de labels van de waarden in de domeinwaardelijst met regelingtypen 
(/join/id/stop/soortregeling), meerdere mogelijk: 
- AMvB - Ministeriële Regeling 
- Omgevingsplan 
- Omgevingsverordening 
- Waterschapsverordening 
- Omgevingsvisie 
- Projectbesluit 
