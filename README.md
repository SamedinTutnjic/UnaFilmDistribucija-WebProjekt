# Booking Management System – UNA Film

## Opis projekta
**Booking Management System – UNA Film** je web aplikacija razvijena s ciljem digitalizacije i automatizacije procesa upravljanja filmskim booking terminima unutar distributerske kompanije **UNA Film d.o.o.**

Sistem omogućava centralizovano upravljanje filmovima, kino partnerima i booking terminima, uz jasno razdvajanje administratorskih i korisničkih ovlasti. Cilj aplikacije je smanjenje manuelnog rada, povećanje tačnosti evidencije i unapređenje efikasnosti poslovnih procesa.

Aplikacija je razvijena isključivo kao web rješenje, dostupno putem web preglednika, bez potrebe za lokalnom instalacijom klijentskog softvera.

---

## Članovi tima
- **Samedin Tutnjić** – Vođa tima / Backend  
 
- **Sanjin Samardžić** – Frontend developer  

- **Kemal Hasanspahić** – Backend / Baza podataka  
 
- **Aldina Ismić** – Frontend / UI  
 
---

## Korisničke uloge i ovlasti
### Administrator
- Upravljanje filmovima
- Upravljanje kino partnerima
- Upravljanje booking terminima
- Pregled i administracija svih podataka u sistemu

### Korisnik (kino partner)
- Kreiranje booking zahtjeva
- Pregled vlastitih booking termina
- Nema administrativne ovlasti

---

## Tehnologije korištene u projektu
- **Frontend:** React (Vite), HTML5, CSS3, JavaScript (ES6+)
- **Backend:** Node.js, Express.js
- **Baza podataka:** MySQL
- **Arhitektura:** REST API
- **Verzionisanje:** GitHub

---

## Funkcionalni zahtjevi
- Upravljanje filmovima (dodavanje, brisanje i pregled)
- Upravljanje kino partnerima (dodavanje, brisanje i pregled)
- Kreiranje, brisanje i pregled booking termina
- Kreiranje booking zahtjeva od strane korisnika
- Autentifikacija korisnika (login)
- Pregled booking termina u kalendarskom prikazu

---

## Nefunkcionalni zahtjevi
- Sigurnost i kontrola pristupa
- Pouzdan i stabilan rad aplikacije
- Brz odziv sistema
- Skalabilnost i mogućnost budućeg proširenja

---

## Pokretanje aplikacije

### Preduslovi
Prije pokretanja aplikacije potrebno je instalirati:
- **Node.js (LTS verzija)**
- **MySQL Server**  
  (MySQL Workbench je opcionalan i služi isključivo za grafički pregled baze)
- Editor po izboru (VS Code, WebStorm i sl.)

> Bez instaliranog i pokrenutog MySQL Servera aplikacija se ne može izvršiti.

---

### Backend – prvo pokretanje (inicijalizacija baze)
Inicijalizacija baze se radi **samo jednom**, prilikom prvog pokretanja projekta na novom računaru.

U terminalu (PowerShell) izvršiti sljedeće komande:

```bash
cd UnaFilmDistribucija/backend
npm install
$env:DB_INIT="true"; npm run dev
````

Ova komanda automatski:

* kreira bazu podataka
* kreira sve potrebne tabele
* ubacuje početne podatke

Kada se u terminalu pojavi poruka:

```
Database initialized successfully
```

potrebno je zaustaviti server (**Ctrl + C**).

---

### Backend – standardno pokretanje

Nakon inicijalizacije baze, backend se pokreće bez ponovnog kreiranja podataka:

```bash
cd UnaFilmDistribucija/backend
npm run dev
```

Backend servis je dostupan na adresi:

```
http://localhost:3000
```

---

### Frontend – pokretanje aplikacije

U novom terminalu izvršiti sljedeće komande:

```bash
cd UnaFilmDistribucija/frontend
npm install
npm run dev
```

Frontend aplikacija je dostupna u web pregledniku na adresi:

```
http://localhost:5173
```

---

## Napomena

Projekat je razvijen u edukativne svrhe u okviru predmeta **Web Programiranje** na Politehničkom fakultetu Univerziteta u Zenici, školska godina **2025/2026**.

---


