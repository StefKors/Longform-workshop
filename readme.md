# Website online zetten
Een website is een map met bestanden op een (server)computer die openbaar zijn gemaakt. De locatie van deze computer is het IP adres bijvoorbeeld `192.30.252.153`. Je kan dit zien als de postcode van de website. Een url is de "straatnaam" Dit is een mooie presentatie van een IP adres.

In de workshop gebruiken wij github om de site te hosten. Dit betekent dat wij onze bestanden beschikbaar gaan maken via de computers van github.

## Install github desktop
Om te beginnen downloaden we github desktop, dit is een handige interface om met github te werken. https://desktop.github.com/

Als hij vraag om 'git' te installeren doe dit dan. Of installeer het via de volgende site:
MAC: https://sourceforge.net/projects/git-osx-installer/files/
Winodws: https://github.com/git-for-windows/git/releases/download/v2.20.1.windows.1/Git-2.20.1-64-bit.exe

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