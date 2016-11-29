---
layout: page
title: "Antwoorden op DDoS aanvallen"
author: RaReNet
language: nl
summary: "Een bedreiging voor veel journalisten, nieuwssites en bloggers is dat hun stem het zwijgen is opgelegd doordat hun website down is of werd gedefaced. In veel gevallen kan dit een vervelend, maar niet minder frusterend probleem zijn. In een aantal gevallen kan het echter het gevolg zijn van een 'denial of service' aanval of een overname van een website. Dit onderdeel van de Digital First Aid Kit helpt je met het doorlopen van een aantal basis stappen om mogelijke problemen vast te stellen. Wanneer uw website onder aanval is kan u hier ook enkele stappen vinden om het probleem op te lossen."
date: 2015-08
permalink: /nl/DDoSMitigation/
parent: /nl/
---

# Antwoorden op DDoS aanvallen

Een bedreiging voor veel journalisten, nieuwssites en bloggers is dat hun stem het zwijgen wordt opgelegd doordat hun website niet meer bereikbaar is of werd gedefaced. In veel gevallen kan dit een onschuldig, maar daarom niet minder frusterend probleem zijn. In een aantal gevallen kan het echter het gevolg zijn van een 'denial of service' aanval of een overname van een website. Dit onderdeel van de Digital First Aid Kit helpt je met het doorlopen van een aantal basis stappen om mogelijke problemen vast te stellen. Wanneer uw website onder aanval is kan u hier ook enkele stappen vinden om het probleem op te lossen.

In het algemeen is het belangrijk om te weten dat er verschillende redenen kunnen zijn waarom uw website niet meer bereikbaar is. In de meeste gevallen is het te wijten aan programmeerfouten of technische problemen bij het bedrijf dat de site host. Soms kunnen andere zaken, zoals bijvoorbeeld een juridisch probleem, aan de oorsprong liggen waarom een hoster uw website uitschakelt. Het vinden van het exacte probleem én daarna de mogelijke oplossingen kan complex en moeilijk zijn als u niet veel ervaring heeft met webhosting. Daarom is het best om, indien mogelijk, als eerste stap iemand te contacteren die u vertrouwt en die u kan helpen met uw website (de webmaster, diegene die uw site heeft gemaakt, uw interne medewerkers -indien u die heeft-, het bedrijf dat uw site host of indien, indien geen enkele van deze aanwezig is, [hulp zoeken bij u een organisatie waar u vertrouwen in heeft](SecureCommunication.md#seeking-and-providing-remote-help) )

Het is een goed gebruik om **de webmaster en uw hoster te contacteren** nadat u enkele van de meer algemene problemen hieronder heeft onderzocht. Uw probleem kan misschien nog niet weergegeven zijn op de statuspagina van uw hoster, het kan een tijdelijk probleem zijn of de hoster heeft het probleem misschien zelf nog niet ontdekt. Een goede verstandhouding met uw leveranciers kan al veel problemen oplossen : wees duidelijk en respectvol en deel de resultaten van uw onderzoek aan de hand van deze vragen. Dit helpt hen verder om het probleem sneller te identificeren.

## Begin met het formuleren van enkele antwoorden op deze basisvragen :

### Algemene informatie

- Wie heeft uw website gemaakt? Zijn deze mensen beschikbaar om u te helpen?
- Wie is uw hoster? Dit is het bedrijf dat de server voorziet waar uw website staat. Indien u dit niet weet kan u daarvoor een [hulpmiddel](http://www.whoishostingthis.com/) gebruiken.
- Heeft u uw login gegevens van uw hosting provider?
- Waar heeft uw de domeinnaam gekocht? In sommige gevallen kan dit ook uw hoster zijn.
- Heeft u uw login gegevens voor de dienst voor het beheren van de domeinnaam? Indien u deze niet meer heeft dan moet het terugvinden van deze gegevens één van uw eerste stappen zijn om uw site te herstellen.
- Zijn er andere mensen die ook toegang hebben tot deze gegevens?


### Diagnose informatie

Er kunnen verschillende redenen zijn waarom uw website niet bereikbaar is. Dit kan gaan van netwerkproblemen tot problemen met de gebruikersovereenkomst, hostingproblemen, blokkering, software, defacement en performantieproblemen. Het volgende deel legt uit wat elk van deze problemen zijn en hoe u zelf kan vaststellen welk probleem u ondervindt.

- **Uw hoster is beschikbaar maar uw website is niet bereikbaar?**
    1. Verifieer dit eerst via [deze website](http://isitdownorjust.me)
        - Uw site is bereikbaar maar u ziet de website niet?
            - Dit is een **netwerk probleem**. Uw eigen internet verbinding kan problemen ondervinden of uw toegang tot uw website is geblokkeerd.
            - Dit zou ook kunnen betekenen dat uw account niet meer beschikbaar of actief is. **Krijgt u een  boodschap van uw hoster te zien?**
                - Uw site kan niet meer beschikbaar zijn omwille van facturatie, juridische, copyright of andere redenen.
                - Dit is een **probleem met de gebruikersovereenkomst**. Zorg dat uw facturatie-gegevens correct zijn en dat er geen openstaand saldo meer is bij uw hosting provider. Indien het een juridisch probleem is kunnen [deze bronnen](https://www.eff.org/issues/bloggers/legal/liability/IP) van EFF, alhoewel toegespitst op de VS copyright wetgeving, een goede start zijn om meer te weten te komen.
        - **Uw site is voor niemand beschikbaar?** Het bedrijf waar u de site host kan problemen hebben. In dit geval heeft u een **probleem met uw hoster**.
            - Kan u de website van uw hoster nog bezoeken? Dit is *niet* het administratie deel van uw website maar de site van het bedrijf of organisatie dat uw site host. Zoek naar de status pagina van uw hoster (bv. status.dreamhost.com); zoek zeker ook op Twitter naar andere boodschappen die over uw hoster gaan.
                - Een simpele zoekactie in Google '(bedrijfsnaam) down' kan u helpen te besluiten of anderen hetzelfde probleem ondervinden.
    2. **Kan u andere websites met gelijkaardige inhoude bezoeken?**
        - Probeer om websites te bezoeken die informatie gelijkaardig aan uw website weergeven. Probeer eventueel ook uw website met [Tor](https://www.torproject.org/projects/gettor.html) of [Psiphon](https://psiphon.ca/products.php) te bezoeken. Indien dit het probleem verhelpt dan heeft u een probleem van **blokkering**. Uw site is nog steeds beschikbaar in andere delen van de wereld maar werd gecensureerd in uw land.
    3. **Ziet u foutboodschappen in uw site?**
        - Dit zou kunnen wijzen op een **software probleem**. Probeer te achterhalen of er recente wijzigingen waren door u of uw team en contacteer uw webmaster.
            - Door een schermafbeelding te sturen naar uw webmaster samen met de link naar de pagina waar u problemen heeft en de foutboodschapen die u ziet kan u samen sneller het probleem vaststellen.
            - U kan eventueel ook via internet zoeken naar de foutboodschappen die u ziet om te onderzoeken of deze misschien eenvoudig zijn te verhelpen.
    4. **Ziet u een andere website dan die van u? Krijgt u een waarschuwing rond malware op uw website?**
        - Dit kan wijzen op een probleem van **defacement**. Zie hierna voor de te nemen stappen; u zal moeten samenwerken met uw hoster en bekijk zeker ook de sectie rond het overnemen van uw account.
    5. **Is uw website traag of moeilijk bereikbaar?**
        - Uw site kan het aantal aanvragen niet meer aan. Dit is een **performantie probleem**. Dit kan 'goed' zijn in de zin dat uw site populairder is geworden en dat u enkel moet zorgen voor wat verbeteringen zodat bezoekers uw site beter / sneller kunnen consulteren.
            - Verifieer de website statistieken (liefst voor een langere periode) en kijk of er een groei is in bezoekers.
            - Vraag uw webmaster of hosting firma voor hulp. Verschillende populaire blog en CMS platformen (Joomla, Wordpress, Drupal en andere) hebben plugins om de site te cachen en te integreren met CDNs. Dit kan een grote -positieve- invloed hebben op de performantie en beschikbaarheid.

## Eerste stappen om het probleem op te lossen

### Wanneer u het slachtoffer bent van een denial of service aanval

Wanneer de bovenstaande diagnose niet helpt (of wanneer u ernstige **performantie problemen** heeft) dan kan uw site mogelijk het slachtoffer zin van een **'denial of service aanval'**. Dit wil zeggen dat een aanvaller (of aanvallers) verschillende keren uw site proberen op te vragen, vaak via geautomatiseerde hulpmiddelen. Op die manier proberen ze de toegang voor 'normale' gebruikers te verhinderen. Soms is het maar één 'aanvaller' en meestal geeft dit niet al te veel problemen, uitgezonderd wanneer u natuurlijk moet betalen voor de bandbreedte van uw site. In de meeste gevallen gaat het echter om een 'Distributed' denial of service, dit wil zeggen dat een aanvaller grote aantallen machines gebruikt om een (uw) website aan te vallen.

- Stap 1: Contacteer iemand die u vertrouwt en die u kan helpen met uw website (uw webmaster, diegene die uw site heeft gemaakt, uw interne medewerkers -indien u die heeft- of het bedrijf dat uw site host).
- Stap 2: Werk samen met het bedrijf waar u de domeinnaam kocht (zoals bijvoorbeeld EasyDNS, [Network Solutions](http://www.networksolutions.com/support/how-to-manage-advanced-dns-records/), [GoDaddy](http://support.godaddy.com/help/article/680/managing-dns-for-your-domain-names)) en verander de 'Time to Live' of TTL naar 1 uur. Dit kan u helpen om uw site sneller op een andere locatie te plaatsen wanneer deze onder aanval is (de standaard waarde is 72 uren of 3 dagen). Heel vaak gaat u deze instelling terug vinden in de 'geavanceerde' instellingen voor uw domein.
- Stap 3: Verplaats uw site naar een dienst die specifiek bescherming geeft tegen DDoS aanvallen. Zie hiervoor bijvoorbeeld [deze lijst ](https://github.com/OpenInternet/MyWebsiteIsDown/blob/master/MyWebsiteIsDown.md#mitigation-services). Enkele opties zijn:
    - [Deflect.ca](https://deflect.ca/)
    - [Google's Project Shield](https://projectshield.withgoogle.com/en/)
    - [CloudFlare's Project Galileo](https://www.cloudflare.com/galileo)
- Stap 4: Zodra u terug controle heeft over uw site moet u uw exacte noden herbekijken en kiezen voor een hosting bedrijf dat meer aandacht heeft voor security. U kan natuurlijk ook kiezen om verder te gaan met het gebruik van de DDoS beschermingsdienst.

### Wanneer u het slachtoffer bent van een defacement aanval

- Stap 1: Verifieer dat dit een ongewenste overname is van uw website. Een spijtige, maar wel perfect legale manier om uw website over te nemen is dat uw domeinnaam is gekocht door iemand anders voor advertentie doeleinden. Zorg er voor dat de betalingen voor uw domeinnaam regelmatig gebeuren en dat het domein niet vervalt en zo kan overgenomen worden door iemand anders.
- Stap 2: Wanneer uw website is gedefaced zorg dat u eerst terug toegang krijgt tot de login van uw website en maak dan zeker een nieuw toegangswachtwoord aan. Zie hievoor ook de sectie rond het overnemen van uw account (Account Hijacking).
- Stap 3: Maak een kopij van de gedefaced website. U kan deze later nodig hebben voor verder onderzoek.
- Stap 4: Sluit uw website tijdelijk af en gebruik een eenvoudige landings-pagina om uw bezoekers te informeren.
- Stap 5: Onderzoek hoe uw website was gehackt. Uw hosting firma kan u hier mee helpen. De meest voorkomende problemen zijn oudere delen van uw site met niet meer onderhouden scripts, verouderde content management systemen of op maat gemaakte programmatie die kwetsbaarheden bevat.
- Stap 6: Herstel de oorspronkelijke site van uw backups. Indien u of uw hosting bedrijf geen backups heeft is het mogelijk dat u uw website helemaal opnieuw moet maken. Wanneer uw backups enkel bij de hosting provider zijn zou het kunnen dat de aanvaller deze backups ook heeft gewist.
- Stap 7: Maak gebruik van een dienst tegen DDoS aanvallen of gebruik een veilige hosting. Deflect.ca kan u helpen in het beschermen van uw sites tegen aanvallen. Cloudflare blokkeert ook verschillende aanvallen. Veilige hosting bedrijven zoals VirtualRoad/Qurium doen ook veel moeite om zulke aanvallen te voorkomen.


## Dit is niet alles! Nog enkele belangrijke stappen

**Wacht niet tot wanneer u onder aanval bent!** De volgende diensten kunnen u snel helpen wanneer u onder aanval bent. Maar u kan uzelf u al beschermen, voor u een aanval moet verduren. Deze maatregelen kunnen u helpen om minder te betalen voor bandbreedte en om uw site online te houden tijdens een aanval. Weet dat het vaak tot drie dagen kan duren voor iedereen u op het internet kan terugvinden op een nieuw, beveiligd, adres. Het is best om voorbereid te zijn en nu al te starten met het nemen van maatregelen.

1. Voor **Veilige Hosting Leverancier** moet u uw website verplaatsen naar hun servers, u verandert immers van hosting provider. Veel van de providers kunnen u helpen in dit proces. Een extra voordeel is dat veel van deze providers nog andere beschermingsmaatregelen aanbieden, naast DDoS bescherming. Een nadeel is natuurlijk de kostprijs (afhankelijk van wat u nu reeds moet betalen) en de controle - u moet de hosting provider vertrouwen omdat zij ook volledige controle hebben over uw website.
    - Voordelen:
        - U heeft één centrale leverancier voor bijna al uw website noden
        - U krijgt beschermingsdiensten voor DDoS, hacking en spam aanvallen
        - Ze voorzien vaak ook in optionele diensten en raadgeving, in sommige gevallen zelfs voor juridische bescherming
        - Een volledig support team om u te helpen
    - Nadelen:
        - U moet de website bij deze partij onderbrengen
        - U moet deze dienst vertrouwen om uw website en rechten te verdedigen
        - Deze diensten zijn vaak duurder (maar u hoeft wel niet meer te betalen voor andere diensten zoals ondermeer DNS)

2. Met **DDoS beschermings diensten** kan u uw site laten waar hij is, u wijzigt enkel de manier dat anderen uw site kunnen bezoeken. Over het algemeen is dit ook eenvoudiger om op te zetten. Deze diensten hebben meestal servers verspreid over de hele wereld die voor u de slechte en ongewenste toegang verwerken. Deze diensten zijn gemakkelijk te configureren en u blijft volledige controle behouden over de website en het beheer van de website. Het vormt vaak wel een uitdaging (zeker voor niet-admin logins en interactieve / javascript omgevingen) om complexe websites achter deze soort 'proxy' diensten te plaatsen. Bespreek dit zeker met uw webmaster, de meeste problemen kunnen immers opgelost worden.
    - Voordelen:
        - Lagere kost (vaak zelfs met een gratis optie)
        - Gemakkelijk en eenvoudig in te stellen
        - U moet niet veranderen van webhosting bedrijf
        - U kan altijd stoppen met de dienst of veranderen van dienst
    - Nadelen:
        - Minder mogelijkheden tot hulp
        - Deze diensten zijn voornamelijk gefocust op DDoS aanvallen en bevatten niet noodzakelijk hulp voor malware of spammers.
        - De SSL (geëncrypteerde) traffiek zal tijdelijk worden ontcijferd en hercijferd door de proxy server.

3. Kies een specifieke provider - voor eender welke dienst moet u een goed gevoel hebben met de leverancier. Dit gaat zowel om vertrouwen in het bedrijf als om ook hun bedrijfsmodel te begrijpen en goed te interpreteren. Is het werkelijk een gratis dienst of betaald u per geleverde prestatie? Wanneer het om een gratis dienst gaat, krijgt u dan minder dienstverlening als bij de betalende versie. Is het ondersteund door de overheid? Het is best om vooraf al zoveel mogelijk informatie te verzamelen om ongewenste verrassingen achteraf te vermijden..

### Stel uzelf deze vraag voor elke dienst :

- Wat is de structuur en ondersteuning van elk bedrijf of organisatie? Welke verificaties of rapportage moeten ze doen?
- Onderzoek in welke andere landen ze ook een juridische vertegenwoordiging hebben en aan welke wetgeving en politionele onderzoeken ze onderhevig zijn.
- Houden ze toegangslogs bij en hoe lang blijven deze dan beschikbaar?
- Hebben ze beperkingen op de inhoud die ze willen hosten en heeft dit een weerslag op uw website?
- Zijn er landen waar ze geen diensten mogen leveren?
- Gebruiken ze een manier van betaling die u ook kan gebruiken? Kan u hun diensten veroorloven?
- Beveiligde communicatie. U moet minstens veilig kunnen inloggen en communiceren met de provider.
- Is er een mogelijkheid tot two-factor authenticatie om de beveiliging van de beheerder-toegang te verhogen? Deze of andere beveiligingsmaatregelen kunnen de dreigingen voor andere vormen van aanvallen op uw website verminderen..
- Welke types van ondersteuning zijn er? Is er een extra kost voor ondersteuning? Gaat u voldoende ondersteuning krijgen bij het gebruik van de gratis dienst?
- Kan u uw website vooraf al eens testen via een soort staging site?

### Vragen voor veilige hosting leveranciers

- Voorzien ze volledige ondersteuning om uw website naar hun diensten te verplaatsen?
- Zijn deze diensten vergelijkbaar of beter dan wat u nu al heeft, zeker op het gebied van hulpmiddelen en diensten? Belangrijke dingen om te verifieren zijn :
    - Een beheerconsole zoals bijvoorbeeld cPanel
    - Email accounts (hoeveel, welke quotas, beschikbaar via SMTP, IMAP)
    - Databases (hoeveel, welke types, welke toegang)
    - Toegang van afstand via SFTP/SSH
    - Ondersteuning voor de programeertalen (PHP, Perl, Ruby, cgi-bin access...) of CMS systemen (Drupal, Joomla, Wordpress…) die uw site gebruikt

### Vragen voor diensten voor beveiliging tegen DDoS aanvallen:

- Wanneer u gebruik maakt van SSL (ook gekend als HTTPS of beveiligde webtoegang), moet u zich afvragen hoe ze deze SSL toegang beheren. In sommige gevallen is het het eenvoudigste indien u uw private SSL sleutel met hun deelt. Wanneer u dit doet moet u uw leverancier sterk vertrouwen omdat zij zich immers ook kunnen voordien als 'uw site'. Hetzelfde probleem stelt zich ook wanneer u kiest voor een soort proxy dienst.
- Stel zeker de nodige vragen hoe ze de toegang tot het beheers-gedeelte en de pagina's voor het aanpasssen van de inhoud beheren en onderhouden.
- Bespreek zeker de interactieve gedeeltes van uw website (gebruikers die inloggen, die commentaar geven, admin/beheer-rechten, complexe interactieve pagina's met javascript of afbeeldignen) - de verschillende proxydiensten beheren dit elk op hun manier; u moet dit zeker onderzoeken vooraleer te veranderen van dienst.

### Specifieke beschermingsdiensten

Specifieke beschermingsdiensten zijn terug te vinden [in deze lijst](https://github.com/OpenInternet/MyWebsiteIsDown/blob/master/MyWebsiteIsDown.md#mitigation-service). Dit is geen volledig overzicht, er zijn ook andere diensten beschikbaar. Maar alle opgelijste diensten zijn reeds een goede manier om te starten omdat ze reeds worden gebruikt door andere leden in de onafhankelijke pers / mensenrechten / vrije meningsuiting gemeenschappen. Zie ook:

- veilige hosting leveranciers:
    - [Qurium (formerly Virtual Road)](https://www.qurium.org/)
    - [The Positive Internet Company](http://www.positive-internet.com/services/vip-hosting)
    - [Greenhost](https://greenhost.net/)

- beveiliging tegen DDoS aanvallen:
    - [Deflect.ca](https://deflect.ca/)
    - [Google's Project Shield](https://projectshield.withgoogle.com/en/)
    - [CloudFlare's Project Galileo](https://www.cloudflare.com/galileo)

## Neem extra maatregelen tegen aanvallers

Zelfs wanneer u nog niet het slachtoffer bent geweest van een een Denial of Service aanval dan kan u deze gids gebruiken om u voor te bereiden en een mogelijke onbeschikbaarheid te verhinderen. Het onderdeel Antwoorden op een Denial of Service Attack](https://github.com/OpenInternet/MyWebsiteIsDown/blob/master/MyWebsiteIsDown.md#responding-to-a-denial-of-service-attack) bespreekt enkele algemene maatregelen die u kan nemen voor een aanval plaats heeft. Het onderdeel Nuttige bronnen geeft u hulp om uw site live te houden. 

- **Backups**: U moet er altijd voor zorgen om regelmatige backups te hebben. Zorg dat u deze backups op een andere plaats dan uw website bewaard. Veel hosters voorzien dit al als een dienst maar het is zeker aan te raden om ook offline kopijen te hebben.
- **Zorg dat uw systeem up to date is**: Wanneer u een Content Management System (CMS) zoals WordPress of Drupal gebruikt moet u er steeds zorg voor dragen om de laatse versie te gebruiken, zeker als er beveiligingsupdates zijn. Wanneer u een eigen gemaakt systeem gebruikt is het misschien beter om over te stappen naar een CMS dat regelmatige updates heeft.
- **Monitoring**: Er zijn verschillende diensten die uw website kunnen monitoren en u een email of bericht sturen wanneer de website niet meer bereikbaar is. [Dit artikel van Mashable](http://mashable.com/2010/04/09/free-uptime-monitoring/) geeft een overzicht van enkele gekende diensten. U moet er u wel van bewust zijn dat het emailadres of telefoonnummer dat u opgeeft u duidelijk associeert met uw website.

## Onderzoek

Wanneer u het slachtoffer bent geweest van een **'Denial of Service'** aanval of van een **Defacement** aanval, dan kan het belangrijk zijn om te onderzoek waarom u het slachtoffer was.

**Waarom bent u aangevallen en waarom net nu?**: Probeer te bedenken wie er baat bij heeft om uw website of organisatie aan te vallen. Heeft u recent iets controversieel gepost? Kan de dreiging gerelateerd zijn aan uw werk of is uw domeinnaam vervallen? Waarom net nu? Kan een recente aanpassing aan uw website de oorzaak zijn van de Denial of Service aanval? Het volgende onderdeel geeft u enkele verwijzingen naar hulp bij digitale noodgevallen en hoe u hier proactief kan op reageren.

## Nuttige bronnen:

- [My Website is Down](https://github.com/OpenInternet/MyWebsiteIsDown)
- [Keep your site alive](https://www.eff.org/keeping-your-site-alive)
- [Security in a Box](https://securityinabox.org/en/chapter_7_2)
- [Threat modeling, Surveillance Self Defense Guide](https://ssd.eff.org/risk/threats)
- [DDoS proactive and reactive measures](https://www.cert.be/files/DDoS-proactive-reactive.pdf)
