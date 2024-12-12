
# **Airbean**
===========

## Decomposition


Vi delade upp sidan i fyra olika huvudkomponenter. Kundhantering, produktkatalog, kassa/betalning och logistik/leverans. 
De huvuddelarna har vi brytit ner i mindre delar för att göra appen och dess delar mer överskådliga. 

Kundhantering tänker vi är en stor del av appen. Här finns mycker information sparade för kunder med konton, som leveransadress, betalningsinformation samt orderhistorik. Inom kundhantering finns även registerning av nya kunder med, samt en del medd kundservice.

Produktkatalogen har vi brytit ner i produktbeskrivningar där information om pris, innehållsförteckning, bilder samt lagerstatus finns mer.

Kassa och betalning är en av huvudfunktionerna i appen, och den är uppdelad i olika delar: kundvagnen, säkerhet, betalningsalternativ samt olika rabatter. 

Inom leverans och logistik tänkte vi mycket på spårningsmöjligheter, där både inloggad och inte inloggad ska kunna spåra sina beställningar. Leveransalternativ är endast drönare, eftersom det är premissen med appen.

## Pattern Recognition

Kunder söker ett enkelt och snabbt sätt att köpa sitt kaffe. Produktkatalogen ville vi därför hålla ganska enkel för att underlätta köpprocessen för kunderna. Appen säljer sex stycken olika produkter och därför kändes både sökfuktion och filtrering överflödiga. För varje produkt i katalogen tänker vi att delar som pris, information, bilder samt lagerstatus är viktiga.

Många användare handlar efter typ av kaffe (ex. cappuccino, latter macchiato), därför tänker vi att det är viktigt att ha tydliga produktrubriker för att göra det enkelt för kunder att snabbt hitta sitt favoritkaffe i menyn. 

Vi tänker att en påminnelse till inloggade kunder som lämnar produkter i kundvagnen kan vara ett bra sätt att få kunder att slutföra sina köp. I dagsläget  är appen ganska lite och straight forward men i utvecklingssyfte tänker vi att det kan vara en bra funktion att ha redan nu.

## Abstraction

Appen är enkelt uppbyggd för att både inloggade och ej inloggade kunder smidigt kan genomföra sina kaffeköp. 
Produktmenyn är appens startsida, och varje produkt har en enkel köpknapp och kundvagnen är lättåtkomlig. Inloggning behöver inte ske förrän man genomför beställningen, vilket gör det enkelt även för kunder utan konto att göra sina köp. Här behövs också en lagringsfunktion (localStorage) för att även ej inloggade kunder ska kunna använda sig av funktionen “spåra din leverans”. 

Appen innehåller mycket information som behöver en lagringsplats, till ex. inloggningsuppgifter och produktinformation. Vi tänker att det är viktigt att använda sig av databaser för att kunna hantera all den informationen. Om en kund vill skapa ett konto behövs användarnamn, lösenord, e-mail, telefonnummer, betalningsinformation samt leveransadress som även de lagras i en databas.

Hantering och validering av viktiga transaktionsdata utan att lagra känsliga detaljer.

## Algorithm Design

- Vi har gjort ett flödesdiagram för en kund som genomför en beställning i appen.
- Kunden landar först på menysidan där kunden kan välja mellan de olika kaffeprodukterna.
- När kunden trycker sig in på en produkt kan hen läsa detaljerna och välja att lägga produkten i kundvagnen eller gå tillbaka till menyn.
- Vill kunden välja produkten får man välja storlek innan man lägger den i kundvagnen. 
- Har kunden handlat klart och tryckt på kundvagnen så är nästa steg att genomföra beställningen.
- Här får kunden välja om hen vill logga in eller inte.  I det steget kan en kund som inte har konto även välja att registerar ett konto.
- Väljer man att inte logga in eller skapa konto får man manuellt välja betalningssätt samt ange leveransinformation.


Länk till Figjam board:
https://www.figma.com/board/kOX4qNLkLIzLDCUwFhY3KH/Datalogiskt-t%C3%A4nkande-Gruppuppgift?node-id=0-1&t=G95sZdBWpJ05ud0X-1 
