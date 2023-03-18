project is UNDER CONSTUCTION

# PublicTransport

Denna uppgift är en möjlighet för den studerande att redovisa för färdigheter i att utveckla skalbara backend tjänster med spring. Projektet är tänkt att återspegla ett industri case där mindre tjänster används i samspel för att skapa större tjänster.

Typiskt finns det 3 större mobilitetskategorier i dagens samhälle som kommer att representera respektive microservice. Enskilt, i grupp eller kommunalt. Tjänsten bygger på att leverera användaren med olika transportalternativ från ovanstående mobilitetskategorier. 

Observera att ruter som ingår i detta program är fiktiva men att det går att inhämta realtidsdata från öppna api:n såsom trafiklabs för tågtrafik, openweather för gå-väder data osv. 

Kategori kommunal transport
Denna kategori hanterar kommunala resvägar. Observera dock att om en plats angivs som inte är en station så bör det anges en promenadrutt till stationen som en del av resvägen.

Precis som i enskilt ska även kommunala rutter gå att favorisera.
Sammanfattning:
I tjänsten för kommunal transport ska det därför finnas endpoints för att:
Hämta kommunal rutt till och från angiven plats
Data som ingår för en rutt är avgångstid, ankomst, byten och restid samt 
Om till eller från plats inte är en station så ska gå-tiden hämtas från api:et som hanterar enskild transport.
Anmäla fel och förseningar
Uppdatera en felanmälan med uppskattad åtgärdad tid.
Hämta fel och förseningar
Om uppskattad åtgärdes tid är angivet så ska detta ingå i svaret.
Om en försening gör så att tiden för en resa överstiger tiden för att promenera (hämtad från api:et som hanterar enskild transport) så ska en gå-rutt föreslås som alternativ resväg.
Markera en rutt som favoriserad
Hämta en lista över favoriserade rutter
Avmarkera en rutt som favoriserad
