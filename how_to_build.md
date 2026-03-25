# Lage din egen GitHub Page – Steg for Steg

En detaljert guide for hvordan du kan lage din egen moderne webside og publisere den som en GitHub Page, akkurat som denne.

---

## Steg 1: Be Copilot Chat om å generere HTML-siden din

### 1.1 Åpne Copilot Chat
- Gå til copilot  eller bruk Copilot direkte i VS Code (som vi installerer senere)
- bruk copilot

### 1.2 Skriv en detaljert prompt
Gi Copilot en klar beskrivelse av hva du ønsker. Eksempel:

```
Lag en moderne, responsiv HTML5-side for et webinar. 
Krav:
- Dark mode design med grønn og blå accentfarger
- Hero-seksjon med stort headinge, meta-informasjon og CTA-knapper
- Outcomes-seksjon som viser hva deltakerne lærer
- Detaljert agenda med nummererte punkter
- Target audience-seksjon
- Organizers-seksjon med kort informasjon
- Footer med links
- CSS inline i <head> - ingen eksterne filer
- Responsiv design (fungerer på mobil, tablet, desktop)
- Moderne animasjoner og hover-effekter
```

### 1.3 Refiner svaret
- Kopier HTML-en du får
- Be Copilot om justeringer hvis noe ikke ser riktig ut
- Eksempel: "Gjør hero-seksjonen større" eller "Legg til flere animasjoner"

### 1.4 Lagre HTML-en
- Kopier all koden og spar den til senere (vi trenger den i Steg 5)

---

## Steg 2: Opprett en GitHub-konto

### 2.1 Gå til GitHub
- Besukt [github.com](https://github.com)
- Klikk **Sign up** øverst til høyre

### 2.2 Fyll ut registreringen
- **E-post**: Bruk en e-post du har tilgang til
- **Passord**: Lag et sterkt passord
- **Brukernavn**: Velg noe som er lett å huske (brukes i GitHub-adresser)
- **Preferences**: Velg "Free" plan (det er gratis!)

### 2.3 Bekreft e-posten
- Du mottar en bekreftelsesmail
- Klikk linken for å aktivisere kontoen

### 2.4 Konfigurer profilen (valgfritt)
- Legg til foto og bio
- Dette vises på din GitHub-profil

---

## Steg 3: Installer Visual Studio Code

### 3.1 Last ned VS Code
- Gå til [code.visualstudio.com](https://code.visualstudio.com)
- Velg din operativsystem (Windows, Mac, Linux)
- Klikk **Download**

### 3.2 Installer
- Åpne filen som ble lastet ned
- Følg installasjons-guiden (bare trykk "Neste" på alle skjermene)
- Velg "Add to PATH" når du blir spurt

### 3.3 Start VS Code
- Klikk "Finish" når installasjonen er ferdig
- VS Code åpner seg automatisk

### 3.4 Installer extensions (valgfritt, men anbefalt)
- Gå til **Extensions** (ikonen på venstre sidebar som ser ut som 4 firkanter)
- Søk etter og installer:
  - **Live Server** (for å se siden i sanntid)
  - **Prettier** (for pent formatert kode)
  - **Git Graph** (for bedre git-oversikt)

---

## Steg 4: Installer Git på PC-en din

### 4.1 Last ned Git
- Gå til [git-scm.com](https://git-scm.com)
- Klikk **Download for Windows** (eller ditt OS)

### 4.2 Installer Git
- Åpne installasjonsfilen
- Følg guiden (bare trykk "Neste" på alle skjermene)
- **Viktig**: Når du blir spurt, velg "Use Git from the command line and also from 3rd-party software"

### 4.3 Konfigurer Git (åpne terminal/PowerShell)

**Windows:**
```powershell
# Åpne PowerShell eller Command Prompt

git config --global user.name "Ditt Navn"
git config --global user.email "din.email@eksempel.no"
```

**Mac/Linux:**
```bash
git config --global user.name "Ditt Navn"
git config --global user.email "din.email@eksempel.no"
```

### 4.4 Verifiser at Git fungerer
```bash
git --version
```
Du bør se en versjonsnummer (f.eks. `git version 2.42.0`)

---

## Steg 5: Opprett repository på GitHub

### 5.1 Logg inn på GitHub
- Gå til [github.com](https://github.com)
- Logg inn med dine nye credentials

### 5.2 Opprett et nytt repository
- Klikk **+** ikonet øverst til høyre
- Velg **New repository**

### 5.3 Fyll ut detaljer
- **Repository name**: Velg et navn (f.eks. `my-webinar-page`)
- **Description**: "Min første webinarside" (valgfritt)
- **Public/Private**: Velg **Public** (så at siden kan vises som GitHub Page)
- **Initialize this repository**: Kryss av **Add a README file**
- Klikk **Create repository**

### 5.4 Noter URL-en
- Du kommer til repository-siden
- URL-en ser ut slik: `https://github.com/brukernavn/my-webinar-page`
- **Kopier denne** – du trenger den snart

---

## Steg 6: Klon repository lokalt

### 6.1 Åpne terminal/PowerShell
**Windows**: 
- Åpne PowerShell
- Naviger til hvor du vil lagre prosjektet:
```powershell
cd C:\Dine\Prosjekter
# eller hvor du ønsker
```

**Mac/Linux**:
```bash
cd ~/Dine/Prosjekter
```

### 6.2 Klon repository
```bash
git clone https://github.com/brukernavn/my-webinar-page.git
cd my-webinar-page
```

Du har nå en lokal kopi av repository-en din!

---

## Steg 7: Lag prosjektet i VS Code

### 7.1 Åpne prosjektet
- Start VS Code
- Gå til **File** > **Open Folder**
- Velg `my-webinar-page`-mappen du nettopp klonte
- Klikk **Select Folder**

### 7.2 Opprett HTML-filen
- Høyreklikk på mappen i venstre sidebar
- Velg **New File**
- Navngi den `index.html`

### 7.3 Lim inn HTML-koden
- Åpne `index.html`
- Lim inn HTML-en du fikk fra Copilot (fra Steg 1)
- **Ctrl+S** (eller **Cmd+S** på Mac) for å lagre

### 7.4 Test siden lokalt (valgfritt)
- Høyreklikk på `index.html`
- Velg **Open with Live Server** (hvis du installerte extensionen)
- Siden åpnes i en nettleser
- Hvis du gjør endringer og lagrer, oppdaterer siden seg automatisk

---

## Steg 8: Commit og push til GitHub

### 8.1 Åpne terminal i VS Code
- Gå til **Terminal** > **New Terminal** (eller **Ctrl+Ø**)

### 8.2 Sjekk status
```bash
git status
```
Du bør se `index.html` som "Untracked files"

### 8.3 Legg til filer
```bash
git add .
```

### 8.4 Lag en commit
```bash
git commit -m "Add webinar landing page"
```

### 8.5 Push til GitHub
```bash
git push origin main
```

Du blir kanskje spurt om å logge inn på GitHub. Følg instruksjonene på skjermen.

---

## Steg 9: Publiser som GitHub Pages

### 9.1 Gå til repository-innstillinger
- På GitHub, åpne ditt repository
- Klikk **Settings** (øverst på siden)

### 9.2 Aktiver GitHub Pages
- Gå til **Pages** (på venstre meny)
- Under **Branch**, velg **main**
- Klikk **Save**

### 9.3 Vent litt
- GitHub hoste siden din automatisk
- Du får en ny URL: `https://brukernavn.github.io/my-webinar-page/`
- Etter få minutter er siden live!

### 9.4 Besøk siden din
- Gå til linken fra Steg 9.2
- Din webinarside er nå online! 🎉

---

## Steg 10: Gjør endringer (når du er klar)

Når du vil oppdatere siden:

1. **Rediger** `index.html` i VS Code
2. **Lagre** (Ctrl+S)
3. **Test lokalt** med Live Server
4. **Commit** og **push**:
   ```bash
   git add .
   git commit -m "Update webinar description"
   git push origin main
   ```
5. Siden oppdateres automatisk på GitHub Pages (etter 30 sekunder - 1 minut)

---

## Tips & Triks

### Lag flere filer
- Du kan legge til `style.css`, `script.js`, etc. hvis du ønsker
- Bare husk å linke dem i `index.html`

### Bruk Live Server
- Lagre og test lokalt før du pusher
- Dette sparer deg for uventede overraskelser

### Sjekk git status ofte
```bash
git status
```
Dette viser alltid hva som er endret og klar til commit

### Gode commit-meldinger
```bash
git commit -m "Add agenda section"  # ✅ Bra
git commit -m "update"              # ❌ Dårlig
```

---

## Troubleshooting

### "fatal: not a git repository"
- Sjekk at du er i riktig mappe: `pwd` (Mac/Linux) eller `cd` (Windows)
- Du skal være i `my-webinar-page`-mappen

### "Permission denied" ved git push
- Logg inn på GitHub når du blir spurt
- Eller generer en personal access token og bruk det som passord

### Siden oppdateres ikke etter push
- Vær tålmodig (det kan ta 1-2 minutter)
- Hard refresh i nettleseren: **Ctrl+Shift+R** (Windows) eller **Cmd+Shift+R** (Mac)

### CSS/bilder vises ikke
- Sjekk at filene er i samme mappe som `index.html`
- Eller bruk relative paths: `./style.css` istedenfor `style.css`

---

## Neste steg: Introduksjon til Agenter

Nå som du har en webinarside live, er du klar for Leksjon 2, hvor vi lærer hvordan du bruker **GitHub Copilot** som din AI-pair programmer 

hva om du ikke gidder å gjøre alle disse stegene? kan en agent gjøre alt dette for meg? 

hint; markdown, agent chat, og helautomatisering

**Stay tuned!** 🚀

---

*Laget for vibecoding-webinaret av EMP Secure og Arrow*
