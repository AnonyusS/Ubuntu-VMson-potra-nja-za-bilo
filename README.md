# Ubuntu-VMson-potra-nja-za-bilo
Ubuntu-VMson-potražnja-za-bilo koju-radnu stanicu
https://assets.ubuntu.com/v1/f401c3f4-Ubuntu_Server_CLI_pro_tips_2020-04.pdf?_ga=2.83651030.1946703254.1635890714-20085913524 https://untu.com/1946703254.1635890714-2008591924/ ://ubuntu.com/appliance/openhab/raspberry-pi Uputstva za instalaciju Ubuntu Windows macOS Šta vam je potrebno MicroSD kartica (minimalno 4GB, preporučljivo 8GB) Raspberry Pi 3 ili 4 Računar sa drajvom za microSD karticu Mikro- USB kabl za napajanje (USB-C kabl za Pi 4) Monitor sa HDMI interfejsom AHDMI kabl za Pi 3 i MicroHDMI kabl za Pi 4 A USB tastaturu Ovi koraci će prebaciti vaš OpenHAB Ubuntu uređaj na vaš Raspberry Pi sa Ubuntu mašinu i omogućiće vam da se prijavite.

Instalirajte Raspberry Pi Imaging Tool Preuzmite alat za obradu slika za Ubuntu

Pripremite microSD karticu Upozorenje Ovo će potpuno izbrisati microSD karticu.

Umetnite microSD karticu u računar Pokrenite snimač slike i kliknite ODABIR OS ODABIR OS Dalje, odaberite Koristi prilagođeno. Odaberite sliku koju ste preuzeli. Prilagođeno Odaberite svoju microSD karticu i kliknite NAPISI. Dok priprema disk, možete prijeći na sljedeći korak i kreirati svoje SSH ključeve za siguran pristup uređaju.

Generiranje ključeva Secure Shell (SSH) Protokol 'Secure Shell' omogućava pristup vašem Ubuntu uređaju i koristi kriptografske ključeve za provjeru autentičnosti uređaja. Potreban vam je SSH softver i ključevi.

Pokrenite sljedeću naredbu:

ssh-keygen -t rsa Ovo pokreće proces generiranja ključeva. Kada izvršite ovu naredbu, uslužni program ssh-keygen traži od vas da naznačite gdje da pohranite ključ. Pritisnite tipku ENTER da prihvatite zadanu lokaciju. Uslužni program ssh-keygen traži od vas pristupnu frazu. Unesite šifru. Sada imate javni i privatni ključ koji možete koristiti za autentifikaciju.

Kreirajte Ubuntu SSO nalog Vaš Ubuntu uređaj će biti dodat na vaš Ubuntu cloud nalog i koristiće vaše SSH ključeve da vas identifikuju. Dodajte svoje ključeve svom nalogu na https://login.ubuntu.com/ssh-keys.

Da biste to učinili, pokrenite sljedeću naredbu u svom terminalu.

mačka ~/.ssh/id_rsa.pub

Kopirajte rezultat u tekstualno polje na web stranici. Kliknite na uvoz i ključ će biti postavljen.

Pokrenite svoj Raspberry Pi sa microSD kartice Sačekajte da se slike Raspberry Pi završe. Uklonite microSD karticu iz računara i umetnite je u Raspberry Pi. Priključite monitor i tastaturu na Pi, koristit ćete ih za početnu konfiguraciju uređaja.

Ako želite da koristite žičanu mrežu, povežite svoj eternet kabl sa Pi pre pokretanja.

Uključite Pi tako što ćete ga povezati na USB napajanje.

Vaš Pi će se pokrenuti i predstaviti vam niz izbora konfiguracije. Morate osigurati da Pi ima pristup internetu kako bi mogao dobiti ažuriranja i provjeriti vaše SSH ključeve. Ako vam je potrebna dodatna pomoć, postoji vodič koji detaljnije prolazi kroz ove korake.

Zatim ćete morati unijeti adresu e-pošte vašeg Ubuntu računa u oblaku. Vaš Pi će se povezati s vašim računom u oblaku i preuzeti vaše SSH ključeve.

SSH u vašem Pi će pokazati ssh naredbu kao što je:

ssh @

Vaše korisničko ime je vaše Ubuntu SSO korisničko ime.

Vaš terminal će vam poželjeti dobrodošlicu u Ubuntu Core.

To je to. Sada kada ste u svom Pi, moći ćete koristiti svoju sliku OpenHAB Ubuntu Appliancea. https://ubuntu.com/appliance/openhab/raspberry-pi https://github.com/canonical/multipass https://ubuntu.com/appliance/openhab https://discourse.ubuntu.com/c/multipass /21?_ga=2.188026088.1946703254.1635890714-2008591924.1635890714
