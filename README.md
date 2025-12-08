# 📅 Budgetprocess Simrishamns kommun 2026–2027

Kalenderfiler och tidplan för budgetprocessen i Simrishamns kommun för budgetåren 2027–2031.

[![Senast uppdaterad](https://img.shields.io/badge/Senast%20uppdaterad-December%202025-blue)]()
[![Licens](https://img.shields.io/badge/Licens-Public%20Domain-green)]()
[![GitHub Pages](https://img.shields.io/badge/Webbsida-Aktiv-success)](https://lundgren9.github.io/budgetprocess_2026/)

## 📋 Innehåll

- [Om projektet](#om-projektet)
- [Filer i repositoryt](#filer-i-repositoryt)
- [Snabbstart](#snabbstart)
- [Användning](#användning)
- [Teknisk information](#teknisk-information)
- [Skillnader mellan filerna](#skillnader-mellan-filerna)
- [Installation i Outlook](#installation-i-outlook)
- [Felsökning](#felsökning)
- [Kontakt](#kontakt)

## 🏛️ Om projektet

Detta repository innehåller kalenderfiler (ICS-format) med alla viktiga datum och händelser i budgetprocessen för Simrishamns kommun för åren 2026–2027. Filerna kan importeras till Outlook, Google Calendar, Apple Calendar och andra kalenderprogram.

**Webbsida:** [https://lundgren9.github.io/budgetprocess_2026/](https://lundgren9.github.io/budgetprocess_2026/)

### Omfattning

Kalendern täcker hela budgetprocessen från:
- **15 december 2025** – KF beslutar om fokusområden
- **12 mars 2026** – Uppstart med budgeten 2027
- **31 januari 2027** – Nämnderna fastställer internbudget

### Viktiga händelser

- ✅ Budgetberedningens möten (investering och drift)
- ✅ Nämndernas deadlines för budgetskrivelser
- ✅ Kommunstyrelsens och kommunfullmäktiges sammanträden
- ✅ MBL-förhandlingar
- ✅ Strategiska utskottets möten
- ✅ Beslut om skattesats och driftbudget

## 📁 Filer i repositoryt

| Fil | Beskrivning | Rekommendation |
|-----|-------------|----------------|
| `index.html` | Webbsida med information och nedladdningslänkar | Besök via GitHub Pages |
| `budgetprocess_2026.ics` | Ursprunglig kalenderfil | För nedladdning och engångsimport |
| `budgetprocess_2026_NY.ics` | Förbättrad kalenderfil med UID och tidszon | ⭐ Rekommenderad för prenumeration |
| `budgetanvisningar.pdf` | Officiellt dokument med tidplan och anvisningar | Källa till kalenderdata |
| `README.md` | Denna fil | Dokumentation |

## 🚀 Snabbstart

### Alternativ 1: Prenumerera (Rekommenderas)

**För automatiska uppdateringar**, prenumerera på kalendern i Outlook:

```
https://raw.githubusercontent.com/lundgren9/budgetprocess_2026/main/budgetprocess_2026_NY.ics
```

**Instruktioner:**
1. Öppna Outlook
2. Gå till: Arkiv → Kontoinställningar → Internetkalendrar → Ny...
3. Klistra in URL:en ovan
4. Klicka OK

### Alternativ 2: Ladda ner och importera

**För engångsimport**, ladda ner filen:

```bash
wget https://raw.githubusercontent.com/lundgren9/budgetprocess_2026/main/budgetprocess_2026_NY.ics
```

Eller klicka på [budgetprocess_2026_NY.ics](budgetprocess_2026_NY.ics) och välj "Download".

## 📖 Användning

### Webbgränssnitt

Den enklaste metoden är att använda vår webbsida:

🌐 **[https://lundgren9.github.io/budgetprocess_2026/](https://lundgren9.github.io/budgetprocess_2026/)**

På webbsidan kan du:
- 📥 Ladda ner kalenderfiler
- 👁️ Visa filinnehållet innan nedladdning
- 🔗 Kopiera prenumerations-URL:er
- 📄 Läsa teknisk dokumentation
- 📑 Öppna budgetanvisningar.pdf

### Direkt nedladdning

**För budgetprocess_2026_NY.ics (rekommenderad):**
```
https://raw.githubusercontent.com/lundgren9/budgetprocess_2026/main/budgetprocess_2026_NY.ics
```

**För budgetprocess_2026.ics (ursprunglig):**
```
https://raw.githubusercontent.com/lundgren9/budgetprocess_2026/main/budgetprocess_2026.ics
```

## 🔧 Teknisk information

### ICS-filformat

ICS (iCalendar) är ett standardformat för kalenderdata definierat i [RFC 5545](https://tools.ietf.org/html/rfc5545).

### Förbättrad version (NY)

`budgetprocess_2026_NY.ics` innehåller följande tekniska förbättringar:

```ics
BEGIN:VCALENDAR
VERSION:2.0
PRODID:-//Simrishamns kommun//Budgetprocess 2026-2027//SV
METHOD:PUBLISH
X-WR-CALNAME:Budgetprocess Simrishamn 2026-2027
X-WR-TIMEZONE:Europe/Stockholm

BEGIN:VTIMEZONE
TZID:Europe/Stockholm
...
END:VTIMEZONE

BEGIN:VEVENT
UID:budgetprocess-2026-03-12-uppstart@simrishamn.se
DTSTAMP:20251208T120000Z
DTSTART;TZID=Europe/Stockholm:20260312T080000
DTEND;TZID=Europe/Stockholm:20260312T120000
SUMMARY:Uppstart med budgeten 2027
DESCRIPTION:Halvdag. Genomgång av tidplan...
LOCATION:Kommunhuset
STATUS:CONFIRMED
END:VEVENT
```

### Nödvändiga fält för prenumeration

För att en ICS-fil ska fungera med kalenderprenumeration krävs:

- ✅ **UID** (Unique Identifier) – Unikt ID för varje händelse
- ✅ **DTSTAMP** (Date-Time Stamp) – Tidsstämpel för skapande/ändring
- ✅ **VTIMEZONE** – Tidszonsinformation (Europe/Stockholm)
- ✅ **METHOD:PUBLISH** – Indikerar publicerad kalender

## 📊 Skillnader mellan filerna

### budgetprocess_2026.ics (Ursprunglig)

**Fördelar:**
- Enklare format
- Fungerar för nedladdning och import

**Nackdelar:**
- ❌ Saknar UID-fält
- ❌ Ingen tidszonsinformation
- ❌ Fungerar INTE för prenumeration via URL
- ❌ Händelser kan visas på fel tid eller inte alls

**Användning:** Endast för engångsimport

### budgetprocess_2026_NY.ics (Förbättrad) ⭐

**Fördelar:**
- ✅ Innehåller UID för varje händelse
- ✅ Korrekt tidszonsinformation (Europe/Stockholm)
- ✅ DTSTAMP för alla händelser
- ✅ Fungerar perfekt för prenumeration
- ✅ Automatiska uppdateringar
- ✅ Korrekt visning av tider
- ✅ Specifika start- och sluttider för möten

**Användning:** Rekommenderad för både import och prenumeration

## 💻 Installation i Outlook

### Nya Outlook

1. Öppna Outlook
2. Gå till kalendervy
3. Högerklicka i kalenderlistan (vänster panel)
4. Välj **"Lägg till kalender"** eller **"+"**
5. Välj **"Prenumerera från webben"**
6. Klistra in URL:
   ```
   https://raw.githubusercontent.com/lundgren9/budgetprocess_2026/main/budgetprocess_2026_NY.ics
   ```
7. Ge kalendern ett namn: "Budgetprocess 2026-2027"
8. Klicka **"Prenumerera"**
9. Vänta 30-60 sekunder – händelser visas automatiskt

### Gamla Outlook (Desktop)

1. Öppna Outlook
2. Gå till: **Arkiv** → **Kontoinställningar** → **Kontoinställningar...**
3. Välj fliken **"Internetkalendrar"**
4. Klicka **"Ny..."**
5. Klistra in URL:en (samma som ovan)
6. Klicka **OK**
7. Ge kalendern ett namn
8. Klicka **OK** igen

### Google Calendar

1. Öppna [Google Calendar](https://calendar.google.com)
2. Till vänster, klicka på **"+"** bredvid "Andra kalendrar"
3. Välj **"Från URL"**
4. Klistra in URL:en
5. Klicka **"Lägg till kalender"**

### Apple Calendar

1. Öppna Calendar-appen
2. Gå till: **Arkiv** → **Ny kalenderprenumeration**
3. Klistra in URL:en
4. Klicka **"Prenumerera"**
5. Justera inställningar om önskat
6. Klicka **OK**

## 🔍 Felsökning

### Problem: Inga händelser visas efter prenumeration

**Lösning:**
1. Vänta 2-3 minuter (kalenderprenumerationer kan ta tid)
2. Högerklicka på kalendern och välj "Uppdatera"
3. Kontrollera att du tittar på **mars 2026 eller senare**
4. Starta om Outlook/kalenderprogram
5. Verifiera att URL:en är korrekt (`raw.githubusercontent.com`)

### Problem: Händelser visas på fel tid

**Lösning:**
1. Använd **budgetprocess_2026_NY.ics** (inte den ursprungliga)
2. Kontrollera att din tidszon i Outlook är satt till **Europe/Stockholm** eller korrekt lokal tidszon
3. Ta bort och lägg till kalendern igen

### Problem: "Not found" eller 404-fel

**Lösning:**
1. Kontrollera att du använder **raw.githubusercontent.com** (INTE github.com)
2. Verifiera att branch-namnet är **main** (inte master)
3. Testa URL:en i webbläsaren först

### Problem: Kan inte ta bort gamla händelser

**Lösning:**
1. Sök efter "budgetprocess" i kalendern
2. Markera alla händelser (Ctrl+A)
3. Tryck Delete
4. Om du har en prenumererad kalender: Högerklicka och välj "Ta bort kalender"





## 🤖 Skapad med AI-assistans

Denna kalender och webbsida har skapats med hjälp av Claude (Anthropic) för att demonstrera hur AI kan assistera med:
- Dataformatering och standardisering (ICS-format)
- Webbutveckling (HTML, CSS, JavaScript)
- Teknisk dokumentation
- Användarupplevelse och tillgänglighet

---

## 🔄 Uppdateringshistorik

### Version 2.0 - December 2025
- ✅ Lagt till UID-fält för alla händelser
- ✅ Implementerat VTIMEZONE för Europe/Stockholm
- ✅ Lagt till DTSTAMP för alla händelser
- ✅ Specificerat start- och sluttider för möten
- ✅ Förbättrad webbsida med modal-funktionalitet
- ✅ Teknisk dokumentation

### Version 1.0 - December 2025
- ✅ Initial version med alla budgetprocessens datum
- ✅ Grundläggande ICS-format
- ✅ Webbsida för nedladdning

---

**⭐ Gillar du projektet? Ge det en stjärna på GitHub!**

📅 **Kalender tillgänglig:** [https://lundgren9.github.io/budgetprocess_2026/](https://lundgren9.github.io/budgetprocess_2026/)
