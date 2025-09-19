# nettverk

Bytta IPen på pien til statisk og pinga den fra laptopen
IP-adressen 10.200.14.28 er en privat adresse i 10.x.x.x-nettverket, som bare brukes internt (for eksempel på skoler, bedrifter eller hjemme), og den kan derfor ikke nås fra internett, men peker på en enhet som en PC, server eller printer i det lokale nettverket.
<img width="945" height="545" alt="image" src="https://github.com/user-attachments/assets/922125f8-1c82-442c-b4cd-e926d10ecced" />


Jeg satte opp en Apache2-server på Ubuntu ved først å oppdatere systemet med sudo apt update && sudo apt upgrade -y. Deretter installerte jeg Apache2 med sudo apt install apache2 -y. Etter installasjonen sjekket jeg statusen med systemctl status apache2 for å være sikker på at tjenesten kjørte, og den stod som active (running). For å teste at det fungerte åpnet jeg en nettleser og skrev inn serverens IP-adresse, og da fikk jeg opp Apache2 sin standard velkomstside. Til slutt prøvde jeg å legge inn en egen HTML-fil i /var/www/html/, og den ble vist i nettleseren, noe som bekreftet at serveren fungerte som den skulle. hvis du ikke putter 800 på slutten så kom det en defult page alle får.

<img width="1856" height="1014" alt="Screenshot From 2025-09-17 11-25-57" src="https://github.com/user-attachments/assets/e51ca723-7fb4-448c-a48d-3071cae4f34f" />

<img width="826" height="583" alt="Screenshot From 2025-09-17 11-26-13" src="https://github.com/user-attachments/assets/e25f3967-8764-4318-8377-e437c6f6ad41" />


Jeg mistet dessverre bildene jeg tok underveis, men sånn gjorde jeg det: Først lagde jeg et lite Python-script på laptopen som bare skriver "Hello world", og lagret det som hello.py. Så opprettet jeg et repo på GitHub og pushet filen dit med vanlige Git-kommandoer.

På Raspberry Pi klonet jeg repoet med git clone og kjørte scriptet med python3 hello.py, og da kom "Hello world" opp i terminalen, så jeg så at det funka.

For å vise push og pull endret jeg litt i scriptet på PC-en, pushet det til GitHub, og kjørte git pull på Raspberry Pi. Da fikk jeg den oppdaterte versjonen der også, og alt fungerte som det skulle.

<img width="1253" height="836" alt="image" src="https://github.com/user-attachments/assets/1fd4c074-b5d8-49f3-8844-86bebac82800" />



