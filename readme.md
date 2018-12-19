# Website online zetten
Een website is een map met bestanden op een (server)computer die openbaar zijn gemaakt. De locatie van deze computer is het IP adres bijvoorbeeld `192.30.252.153`. Je kan dit zien als de postcode van de website. Een url is de "straatnaam" Dit is een mooie presentatie van een IP adres.

In de workshop gebruiken wij github om de site te hosten. Dit betekent dat wij onze bestanden beschikbaar gaan maken via de computers van github.

## Verklarende woordenlijst

- Git: Versie beheersysteem
- GitHub: een van de vele websites om samen te werken met git projecten
- GitHub Desktop: een programma die het makkelijker maakt om met git te werken. Een alternatief is de terminal gebruiken.
- Repository: De folder die opgenomen is in het git systeem
- Commit: Een 'save' van de huidige staat van de folders
- Push/Pull: de manier om de folder op de server en de folder op jouw computer up to date te houden. (je duwt/push jouw wijzinging naar de server)
- GitHub Pages: de feature waarmee je de bestanden in het git versie systeem beschikbaar kan maken via een url
- IP adress: de 'postcode' van de server
- Url: het mooie adres van jouw website
- Domein: het onderdeel van de url tussen `www` en `/index.html`
- DNS: Het telefoon boek die bijhoud welk domein bij welk IP adres hoort.

## Installeer Github Desktop
Om te beginnen downloaden we Github Desktop, dit is een handige interface om met GitHub te werken. https://desktop.github.com/

Als hij vraag om 'git' te installeren doe dit dan. Of installeer het via de volgende site:
- MAC: https://sourceforge.net/projects/git-osx-installer/files/
- Winodws: https://github.com/git-for-windows/git/releases/download/v2.20.1.windows.1/Git-2.20.1-64-bit.exe

## Maak een account bij GitHub
Via de volgende link kan je een account aanmaken. Kies het gratis account.
https://github.com/join?source=experiment-header-dropdowns-home

## GitHub Desktop gebruiken
1) Open github desktop
2) Login
3) Ga naar: `File > New Repository`
4) Geef het een naam
5) Selecteer een nieuwe folder
6) Klik "Create Repository"
7) Zet je longform file in de folder via finder/explorer
8) In github desktop 
9) Klik bovenin "Publish Repository"
10) Klik bovenin "Publish Repository"
11) Ga naar: `Repository > View on Github`

## Site publiek maken
1) Op github ga naar Settings
2) Bij het kopje "Github Pages" zet de dropdown naar `master branch`
3) Klik `save`
4) Scroll naar beneden en klik op de url
5) 🎉🎉 Je website is live! 🎉🎉

## (sub)Domein instellen
1) Ga naar DNS beheer
2) Stel de volgende waarden in:

| Value 					| Type	| Value					|  TTL 	| 
|---						|---	|---					|---	|
|  stefkors.com 			| A  	|  192.30.252.154 		|  1uur	| 
|  stefkors.com 			| A  	|  192.30.252.153 		|  1uur	| 
|  longform.stefkors.com 	| CNAME	|  stefkors.github.io. 	|  1uur	| 

3) Voeg een bestand toe aan je folder op de computer met de naam `CNAME` en als content je sub domein bijvoorbeeld `longform.stefkors.com`
4) Via het github Desktop programma `commit` en `push` het nieuwe bestand via de zij-balk en de klop aan de bovenkant.
5) Op github ga je naar de settings van je repository
6) Bij het kopje "Github Pages" zet het custom domein naar `longform.stefkors.com`
7) Wacht tot alle wijzingen zijn doorgevoegd. Dit kan 5minuten tot 4uur duren. (meestal gaat het vrij snel)
8) 🎉🎉 Je website is live op je eigen domein! 🎉🎉







https://help.github.com/articles/using-a-custom-domain-with-github-pages/