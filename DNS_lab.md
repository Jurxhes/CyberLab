DNS in Detail – TryHackMe Lab
Obiettivo del lab:
Comprendere come funziona il sistema DNS, dai record base alla risoluzione dei nomi in indirizzi IP, e capire le differenze tra record A, CNAME, MX e PTR.
Strumenti usati:
Browser + TryHackMe platform
Comandi di terminale: nslookup, dig
Annotazioni personali
Concetti chiave imparati:
Cos’è il DNS: sistema che traduce nomi di dominio leggibili in IP numerici.
Record principali:
A → indirizzo IPv4
AAAA → indirizzo IPv6
CNAME → alias di un altro dominio
MX → record per email
PTR → record inverso (IP → dominio)
Funzionamento della risoluzione:
Il resolver chiede al DNS server locale
Se non sa la risposta, contatta i server root → TLD → authoritative
Esempi pratici provati nel lab:
nslookup example.com → restituisce indirizzo IP
dig +short example.com A → output chiaro dell’IP
Analisi dei record MX per gmail.com
Riflessione personale:
Ho capito che il DNS è la base di tutta la comunicazione web. Sapere leggere i record e capire come funzionano le query è fondamentale anche per capire possibili vulnerabilità (DNS spoofing, cache poisoning, ecc.).
