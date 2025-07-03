# 👨‍💻 Gruppövning: Agilt Arbetsflöde med Scrum och Git

Denna övning är designad för att ni i grupp ska få praktisk erfarenhet av de agila principerna, Scrum-processen och hur ni samarbetar effektivt med Git, Pull Requests och Code Reviews.

---

## 🎯 Mål med Övningen

- **Förstå processen**: Få en känsla för ett agilt arbetsflöde och hur Scrum-koncept tillämpas.  
- **Praktisera Git-samarbete**: Använda Git för att hantera feature branches, skapa Pull Requests (PRs) och genomföra Code Reviews.  
- **Kommunikation**: Öva på att kommunicera och samarbeta effektivt i ett utvecklingsteam.  
- **Verktyg**: Få en introduktion till att använda GitHub Projects för att hantera ert arbete.  

---

## 👥 Gruppstorlek

Arbeta i grupper om **3–4 studenter**.

---

## 💡 Projektbeskrivning: Enkel studentkatalog

Ni ska tillsammans bygga en enkel webbapplikation för att visa en lista över studenter med grundläggande information.

- **Typ**: Statisk HTML-sida med dynamiskt innehåll via TypeScript.  
- **Fokus**: Förstå och tillämpa arbetsflödet – applikationens komplexitet är sekundär.  
- **Tekniker**: HTML, CSS, TypeScript, Git/GitHub.

---

## 🚀 Arbetsflöde (simulerad sprint)

### Steg 1: Projekt- och Git-Initiering

_Görs av en person per grupp_

1. **Skapa nytt GitHub-repository**  
   - Exempel: `studentkatalog-agile-gruppX`
2. **Initiera grundprojektet**
   - `index.html` (tom `<body>`, länk till TypeScript-fil)  
   - `style.css` (tom)  
   - `src/main.ts`  
   - `tsconfig.json`
3. **Lägg till HTML-struktur**  
   - `<h1>` och en tom `<div>` för studentlistan
4. **Initial commit**
   - Commit och push till `main`
5. **Bjud in gruppmedlemmar** som "Collaborators"
6. **Klona repot** lokalt för övriga gruppmedlemmar

---

### Steg 2: Sprint Planning

_Görs av hela gruppen_

1. **Skapa GitHub Project Board**  
   - Använd "Basic Kanban"-mall
2. **Skapa User Stories som Issues**

#### User Stories:

- **US1: Visa studentnamn**  
  _Som en användare vill jag se en lista med studenters namn på webbsidan._  
  _(Visa minst 3 studenter, hårdkodade i TypeScript-koden.)_

- **US2: Visa studentålder**  
  _Som en användare vill jag se åldern för varje student bredvid deras namn._  
  _(Uppdatera studentobjekten och DOM-manipulation.)_

- **US3: Markera aktiv status**  
  _Som en användare vill jag se om en student är aktiv i kursen._  
  _(Lägg till `isActive: boolean` och visa visuellt med CSS/DOM.)_

- **US4: Lägg till ny student (knapp)**  
  _Som en användare vill jag kunna klicka på en knapp för att lägga till en ny student._  
  _(Använd event listener i TypeScript.)_

3. **Tilldela Issues**  
   - Tilldela personer till respektive Issue  
   - Flytta till "In Progress" på Project Board vid start

---

### Steg 3: Feature Development

_För varje User Story_

1. **Skapa feature branch**
   ```bash
   git checkout main
   git pull origin main
   git checkout -b feature/min-user-story
````

2. **Implementera funktionalitet**

   * TypeScript, HTML, CSS
   * Kompilera (`tsc`) och testa regelbundet

3. **Committa ändringar**

   ```bash
   git add .
   git commit -m "USX: Beskrivande commitmeddelande (#Issue-nummer)"
   ```

4. **Pusha feature branch**

   ```bash
   git push origin feature/min-user-story
   ```

5. **Uppdatera Project Board**

   * Flytta Issue till "In Review"

---

### Steg 4: Pull Request (PR) & Code Review

1. **Skapa Pull Request (PR)**

   * Från feature branch → `main`
   * Titel: t.ex. `US1: Implementera visning av studentnamn`
   * Beskriv innehållet
   * Länka till Issue via `Closes #<nummer>`
   * Tilldela minst en reviewer

2. **Genomför Code Review**

   * Granska kod, kommentera
   * Föreslå förbättringar eller påpeka buggar
   * Godkänn PR när du är nöjd

3. **Åtgärda feedback**

   * Uppdatera feature branch, commit och push igen

4. **Merge PR**

   ```bash
   git checkout main
   git pull origin main
   git merge feature/din-feature-branch
   git push origin main
   git branch -d feature/din-feature-branch
   ```

   * Ta bort feature-branchen på GitHub

5. **Uppdatera Project Board**

   * Flytta Issue till "Done"

---

### Steg 5: Presentation (fredag)

* **Presentera processen**

  * Arbetsfördelning
  * Användning av Git & PR
  * GitHub Projects
  * Code Review-erfarenheter
  * Utmaningar och lösningar
* **Visa er studentkatalog** (även om den är enkel!)

---

## 🛎️ Viktiga påminnelser

* **Kommunicera!**
* **Små, frekventa commits**
* **Testa ofta**
* **Fokusera på processen, inte perfektion**
* **Fråga om hjälp om ni kör fast**

---

**Lycka till! 🚀**

