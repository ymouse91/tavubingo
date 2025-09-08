# Tavubingo

Tavubingo on suomenkielinen **tavupohjainen bingo**. Pelaajilla on **3×3-ruudukko**, joka täytetään tavuilla sanalistasta. Pelin vetäjä arpoo sanoja, ja kun sanasta löytyvät ruudukossa esiintyvät tavut, pelaaja merkitsee ne ruudukkoonsa. Bingo syntyy, kun vaakaan, pystyyn tai diagonaaliin kertyy kolme merkintää.

---

## Tiedostot

- **index.html** – pääsivu, joka avataan selaimessa. Sisältää 3×3-ruudukon ja pelilogiikan.
- **manifest.json** – PWA-asetukset (nimi, ikonit).
- **service-worker.js** – välimuistitus ja offline-tuki.
- **sanat_s2.txt** – tavutettu sanalista (täydellinen).
- **sanat_s2_simple.txt** – yksinkertaistettu sanalista.
- **icons/** – sovelluksen ikonit eri kokoisina.

---

## Pelin säännöt

1. Jokaiselle pelaajalle arvotaan 3×3-tavuruudukko sanalistasta.
2. Vetäjä arpoo sanoja tiedostosta `sanat_s2.txt` (tai `sanat_s2_simple.txt`).
3. Pelaajat merkitsevät ruudukkoonsa ne tavut, jotka esiintyvät arvotussa sanassa.
4. **Bingo!** – kolme merkintää vaakaan, pystyyn tai diagonaaliin riittää voittoon.
   - Vaihtoehtoiset pelimuodot: useampi bingo tai koko ruudukon täyttö.

---

## Käyttö

Avaa `index.html` selaimessa:

- Suoraan: kaksoisklikkaa tiedostoa → aukeaa selaimeen.
- Paikallisen palvelimen kautta (suositus, sama kuin GitHub Pages):
  ```bash
  python -m http.server 8000
  ```
  → selaa osoitteeseen `http://localhost:8000/`

---

## Julkaisu

Projektin voi julkaista **GitHub Pagesissa**:
1. Työnnä repo GitHubiin.
2. Mene *Settings → Pages* ja ota käyttöön `main`-branch.
3. Sovellus on saatavilla osoitteessa `https://<käyttäjä>.github.io/<repo>/`.

---

## Lisenssi

MIT (ks. `LICENSE`).
