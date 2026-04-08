# Specifikacija zahtev za program lojalnosti Maestro

Anže Barle Čuk

## 1. Kratek opis sistema
Sistem lojalnosti trgovske verige Maestro je namenjen spodbujanju strank k večjim in pogostejšim nakupom. Rešitev omogoča strankam zbiranje točk zvestobe na podlagi mesečne porabe, pri čemer so nagrajene glede na svoj nivo lojalnosti. Sistem vključuje varno spletno registracijo, uporabniški portal za pregled stanja in administrativni del za upravljanje pravil.

---

## 2. Funkcionalne zahteve (FZ)
Funkcionalne zahteve opredeljujejo ključne storitve, ki jih mora sistem zagotavljati:

* **FZ-01: Spletna registracija:** Stranka se lahko registrira prek spleta z vnosom osebnih podatkov.
* **FZ-02: Varna verifikacija:** Sistem mora preprečiti registracijo z uporabo tujega elektronskega naslova.
* **FZ-03: Upravljanje statusov:** Sistem mora avtomatsko razvrščati stranke v nivoje: Osnovni, Bronasti, Srebrni in Zlati.
* **FZ-04: Mesečni izračun točk:** Točke se izračunajo enkrat mesečno na podlagi zneska nakupov iz poslovnega IS.
* **FZ-05: Dinamična pravila:** Administrator mora imeti možnost spreminjanja pragov za točke in pogojev za prehode med statusi.
* **FZ-06: Uporabniški portal:** Člani lahko pregledujejo točke, koristijo ugodnosti in vidijo zgodovino zneskov nakupov.
* **FZ-07: Administracija:** Omogoča statistiko nakupov, poljubne poizvedbe po bazi in upravljanje nagradnega programa.

---

## 3. Nefunkcionalne zahteve (NFZ)
Lastnosti sistema, ki zagotavljajo kakovostno delovanje:

* **NFZ-01: Skalabilnost:** Sistem mora podpirati vsaj 500.000 uporabnikov z možnostjo širitve na tuje trge.
* **NFZ-02: Večjezičnost:** Celotna podpora mora biti na voljo v slovenščini in angleščini.
* **NFZ-03: Tehnološka osnova:** Za shranjevanje podatkov se uporabi obstoječa Oracle podatkovna baza.
* **NFZ-04: Intuitivnost:** Uporabniški vmesnik mora biti sodoben in enostaven za uporabo.
* **NFZ-05: Varnost:** Dostop do portala je mogoč le prek uporabniškega računa, ustvarjenega ob registraciji.

---

## 4. Vmesniki za delovanje
Sistem za svoje delovanje potrebuje povezave z naslednjimi zunanjimi sistemi:

* **Poslovni IS Maestro:** Vmesnik za pridobivanje podatkov o opravljenih nakupih strank.
* **E-poštni sistem:** Za varno potrjevanje registracije in komunikacijo z uporabniki.
* **Logistični vmesnik:** Sistem za generiranje podatkov za pošiljanje fizičnih kartic lojalnosti po pošti.
* **Oracle DB:** Neposreden dostop do baze za shranjevanje statusov, točk in pravil.

---

## 5. Slovar zahtev (Glossary)

| Izraz | Opis |
| :--- | :--- |
| **Nivo lojalnosti** | Stopnja zvestobe (Osnovni, Bronasti, Srebrni, Zlati), ki določa ugodnosti. |
| **Točkovnik** | Pravila za dodeljevanje točk glede na znesek nakupa in status. |
| **Portal** | Spletna aplikacija za stranke in administratorje. |
| **Poslovni IS** | Obstoječ informacijski sistem, ki beleži transakcije nakupov. |
| **Prehajanje statusov** | Avtomatska sprememba nivoja stranke na podlagi nakupnega obnašanja. |

<img width="862" height="558" alt="plant" src="https://github.com/user-attachments/assets/b1dc9a12-c1d5-4aa7-8535-5a9abe5784cd" />

## 6.Funckijska dekompozicija
<img width="1674" height="586" alt="image" src="https://github.com/user-attachments/assets/1d5a216b-6a1b-443a-8f34-ac348456e7b0" />

## 7.Funkcionalni model
<img width="1598" height="668" alt="image" src="https://github.com/user-attachments/assets/c95ea082-e948-405e-ad2c-81577e35d5ef" />

## 8.Uporabniski tokovi
<img width="375" height="820" alt="456" src="https://github.com/user-attachments/assets/2c05fac3-9ab5-4c10-afc1-43d14c8dce46" />

