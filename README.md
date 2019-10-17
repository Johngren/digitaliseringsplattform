# Region Östergötlands Digitaliseringsplattform (RÖD)

Här håller vi på att bygga upp information till utvecklare och andra som är intresserade av att skapa system och applikationer som via  Region Östergötlands Digitaliseringsplattform (RÖD) interagerar med de komponenter och system som finns i regionen. API-inventering och beskrivning pågår och så småningom flyttas sannolikt informationen till en "riktig" utvecklingsportal.

## Bakgrund och information om RÖD
* Presentationer
* Strategi- och arkitektur-dokument
...

## Inloggning & Access
* Applikationer kan via vår "IDP" och "API-gateway" låta användare logga in via BankID, vårdens etablerade eTjänste/SITHS-kort+PIN, användarnamn+lösen m.m. beroende på hur man väljer att konfigurera för den specifika applikationen. Applikationsutvecklarens kod behöver bara kunna hantera "biljetter" via OAUTH2*, så sköter vår IDP resten av inloggning etc.

## Tillgängliga API:n och komponenter
* Strukturerad Vårdinformation [openEHR](https://www.openehr.org/)* via Better Plattform, se https://www.ehrscape.com/ för API
* Filöverföring/lagring [FileCloud](https://www.getfilecloud.com/developer/)** och WebDAV* (via FileCloud)
 
## API:n och komponenter på gång
* DICOM* Worklists (Går att koppla till journalsystemet Cosmic och PACS)
* Bild- och filmhantering (inkl. mellanlagring) via VidiView**, flöden kan kopplas till PACS för permanent lagring.
* Skicka SMS
* ...

## Öppna data
Många av ovanstående tjänster kan innehålla persondata och kräver inloggning, anonymiserade Öppna Data finns istället under https://www.regionostergotland.se/psidata/

Saker markerade med * ovan baserar sig på (internationella) öppna standarder eller specifikationer
Saker markerade med ** ovan har utöver API tillhörande klientmjukvara (ivbalnd även mobilapplikation) som är tillgägnlig för regionmedarbetare och kan tillgängliggöras för samarbetspartners
