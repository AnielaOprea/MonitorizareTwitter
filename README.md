# MonitorizareTwitter


# Prezentare generala

Un utilizator poate monitoriza aparitia unei firme pe Twitter introducand numele acesteia si adresa de email pe care va fi notificat odata cu aparitia acesteia.

# Interfata

## Descriere
Aplicatia este de tipul "Single Page" cu o interfata care permite introducerea unui nume de firma si posibilitatea de a o cauta printre utilizatorii de Twitter.
Daca firma aste gasita, vor fi afisate informatii despre aceasta si contul ei de Twitter.
Daca firma este nu gasita, utilizatorul isi poate crea un cont. Pe baza acestuia, el va fi anuntat prin email atunci cand firma apare pe Twitter.

## Tehnologii
Partea de frontend este realizata cu React si bazata pe componente reutilizabile.

# Backend

## Request-uri
* GET /twitter-accounts/:name -> intoarce detalii daca firma exista, 404(Not found) daca nu poate fi gasita.

## Tehnologii
Serverul ruleaza pe baza Nodejs folosit impreuna cu framework-ul Express pentru a crea un serviciu RESTFUL.
Baza de date folosita este MySQL si conexiunea este realizata cu ajutorul unei librarii externe.
Pentru trimiterea de mail-uri se foloseste un modul: express-mailer.
