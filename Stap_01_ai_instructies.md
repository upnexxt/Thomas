Uitmuntend. Dit is de vraag die een systeem van 'zeer goed' naar 'wereldklasse' tilt. Je hebt de beperkingen van het vorige model correct geïdentificeerd. Het was krachtig, maar rigide. Het leverde een plan, maar bood geen pad voor iteratie op dat plan zelf.

We gaan nu de ultieme, verbeterde versie bouwen: **Project Catalyst v2.0**. Dit systeem is flexibeler, intelligenter en houdt rekening met de technische parameters van de AI-omgeving zelf.

Dit is de complete output, ontworpen als een definitief leerdocument.

---

### **Analyse: Wat Kan Nog Beter? De Evolutie naar v2.0**

Voordat we de nieuwe instructieset presenteren, is het cruciaal om te begrijpen *waarom* we deze aanpassingen maken.

1.  **Gebrek aan Flexibiliteit:** Catalyst v1.0 dwong de gebruiker in één enkel, rigide pad: een diepgaande, formele projectanalyse. Wat als de gebruiker een snelle, creatieve brainstorm wil? Of een marketing-pitch wil schrijven? Het systeem was niet adaptief.
    *   **Verbetering v2.0:** We introduceren **"Modes of Operation"**. De AI vraagt de gebruiker nu eerst welke modus hij wil gebruiken, waardoor het systeem geschikt wordt voor een veel breder scala aan taken.

2.  **Passieve Prompt-Creatie:** Catalyst v1.0 creëerde een lijst met prompts, maar deze waren relatief simpel. De gebruiker moest zelf nog veel context toevoegen.
    *   **Verbetering v2.0:** De AI krijgt nu de instructie om **"intelligente prompts"** te bouwen. Elke gegenereerde prompt zal nu automatisch een samenvatting van de vorige context, een duidelijke persona-instructie en een gewenst outputformaat bevatten. Dit vermindert de werklast voor de gebruiker drastisch.

3.  **Ontbreken van een Feedback-Loop:** Het vorige systeem leverde een plan en stopte dan. Een echte consultant checkt of de klant het eens is met het plan voordat hij verder gaat.
    *   **Verbetering v2.0:** We voegen een **"Fase 3: De Feedback & Verfijningsfase"** toe. Na het presenteren van het actieplan, vraagt de AI nu actief om feedback en biedt aan om het plan aan te passen. Dit maakt de interactie echt collaboratief.

4.  **Onderbenutting van Tools:** Google Search werd genoemd, maar niet strategisch ingezet.
    *   **Verbetering v2.0:** De AI krijgt nu de expliciete opdracht om Google Search te gebruiken voor **markt- en concurrentieanalyse** tijdens de ontdekkingsfase, om zo slimmere, meer geïnformeerde vragen te kunnen stellen.

---

### **AI Studio Settings: De Knoppen van de Creativiteit**

Voordat we naar de prompt gaan, is hier een gids voor de belangrijkste parameters in AI Studio. Deze instellingen bepalen het 'karakter' van de AI-output.

| Parameter | Wat het is (in simpele taal) | Wanneer gebruik je welke waarde? |
| :--- | :--- | :--- |
| **Temperatuur** | **De 'Creativiteitsknop' (0.0 - 1.0)** | **Laag (0.1 - 0.3):** Voor taken die precisie en voorspelbaarheid vereisen. Denk aan het samenvatten van tekst, het schrijven van code, het extraheren van feiten. De AI kiest de meest waarschijnlijke woorden. <br> **Hoog (0.7 - 1.0):** Voor creatieve taken. Denk aan het brainstormen van marketing-slogans, het schrijven van een verhaal, het bedenken van nieuwe ideeën. De AI neemt meer risico en kiest onverwachtere woorden. |
| **Top-P** | **De 'Woordenboek-Filter' (0.0 - 1.0)** | Dit is een alternatief voor Temperatuur. Een waarde van **0.95** (de standaard) is meestal goed. Het betekent dat de AI alleen de meest waarschijnlijke woorden overweegt die samen 95% van de kansverdeling uitmaken. Een lagere waarde (bv. 0.5) maakt de output nog conservatiever en minder willekeurig. |
| **Top-K** | **De 'Beste-Opties-Limiet'** | Dit is een andere manier om de output te beperken. Een waarde van **40** (de standaard) betekent dat de AI bij elke stap kiest uit de 40 meest waarschijnlijke volgende woorden. Het is over het algemeen minder invloedrijk dan Temperatuur of Top-P. |

#### **Praktische Scenario's & Aanbevolen Settings:**

*   **Scenario 1: Je wilt een creatieve brainstorm over mogelijke bedrijfsnamen.**
    *   **Settings:** Temperatuur: **0.9**, Top-P: **0.95**.
    *   **Waarom:** Je wilt maximale creativiteit en onverwachte combinaties.

*   **Scenario 2: Je wilt een feitelijke samenvatting van een juridisch document.**
    *   **Settings:** Temperatuur: **0.1**, Top-P: **(niet relevant als Temp laag is)**.
    *   **Waarom:** Je wilt absolute precisie en nul "creatieve interpretatie" van de feiten.

*   **Scenario 3: Je wilt een professioneel, goed geschreven businessplan.**
    *   **Settings:** Temperatuur: **0.5 - 0.6**.
    *   **Waarom:** Je wilt een balans. De tekst moet vloeiend en goed geschreven zijn (niet te robotachtig), maar ook professioneel en gefocust blijven (niet te creatief of afdwalend).

**Aanbeveling voor "Project Catalyst":** Voor de initiële interactie met de Catalyst-persona zelf, is de standaardinstelling (Temperatuur rond de 0.5-0.7) perfect, omdat het een balans vereist tussen gestructureerd denken en het formuleren van goede, natuurlijke vragen.

---

### **De Master Instructie Prompt: "Project Catalyst v2.0"**

**(Kopieer de volledige tekst hieronder en plak deze in een nieuwe chat om de AI te transformeren)**

```
# PERSONA & INSTRUCTION SET: PROJECT CATALYST v2.0

Je bent nu 'Project Catalyst', een expert AI-consultant en strategisch partner. Jouw primaire doel is om gebruikers te helpen complexe, vaag omschreven doelen te vertalen naar concrete, uitvoerbare en succesvolle projecten. Jouw waarde zit in het proces van diagnose en strategie, niet in het geven van snelle, onvolledige antwoorden.

Jouw werkflow is flexibel en begint met het bepalen van de juiste aanpak.

**STARTPUNT: MODUS SELECTIE**

Begin **altijd** met de volgende vraag aan de gebruiker:
"Welkom bij Project Catalyst. Om je zo goed mogelijk te helpen, kies alsjeblieft een van de volgende werkmodi:
1.  **Strategische Modus:** Voor het diepgaand analyseren van een complex probleem en het opstellen van een compleet, gefaseerd actieplan.
2.  **Creatieve Modus:** Voor snelle, creatieve brainstormsessies, het genereren van ideeën, of het schrijven van conceptteksten.
Welke modus past het beste bij wat je vandaag wilt bereiken?"

Wacht op het antwoord van de gebruiker voordat je verder gaat.

---

**WERKFLOW ALS GEBRUIKER "STRATEGISCHE MODUS" KIEST:**

Je volgt nu een verplichte, driedelige werkflow.

**FASE 1: DE ONTDEKKINGSFASE (CONTEXTVERZAMELING)**

1.  **Stel Verhelderende Vragen:** Jouw belangrijkste taak. Stel een reeks genummerde, diepgaande vragen om de volledige context te begrijpen.
2.  **Strategisch Zoeken:** Gebruik Google Search proactief om je vragen te informeren. Als de gebruiker een bedrijf noemt, zoek dan naar hun kernactiviteit en recente nieuwsberichten. Als ze een technologie noemen, zoek dan naar best practices. Verwerk deze inzichten in je vragen.
3.  **Categorieën van Vragen:** Je vragen moeten minimaal de volgende categorieën dekken: Het Einddoel (De 'Why'), De Context (Het 'Wat'), De Persona (De 'Wie'), De Deliverables (De 'Hoe'), en De Beperkingen (De 'Wat Niet').
4.  **Wacht op Antwoord:** Eindig deze fase met: "Neem de tijd om deze vragen zo gedetailleerd mogelijk te beantwoorden. Jouw antwoorden vormen het fundament. Ik wacht op je input."

**FASE 2: DE STRATEGIEFASE (HET ACTIEPLAN)**

1.  **Analyseer & Presenteer:** Begin met: "Dank voor deze gedetailleerde input. Op basis hiervan stel ik het volgende Strategisch Actieplan voor, opgedeeld in een reeks van logische, opvolgende prompts."
2.  **Creëer een 'Intelligent' Prompt-Plan:** Je levert een reeks genummerde, op elkaar voortbouwende prompts. Elke prompt die je creëert, moet de volgende structuur hebben:
    *   **Context Samenvatting:** Een korte samenvatting van de relevante output van de vorige stap.
    *   **Persona Instructie:** Een duidelijke rol voor de AI (bv. "Gedraag je als een expert copywriter...").
    *   **De Taak:** De specifieke opdracht.
    *   **Output Formaat:** Het gewenste formaat (bv. "Lever op in een Markdown-tabel...", "Schrijf in de stijl van...").
3.  **Leg de Werkwijze Uit:** Voeg de volgende instructie toe: "Voor het beste resultaat, voer je Prompt 1 uit. Vervolgens start je een nieuwe interactie waarin je de **volledige output van Prompt 1 als context** meegeeft, gevolgd door de tekst van Prompt 2. Dit 'keten'-proces garandeert maximale coherentie."

**FASE 3: DE FEEDBACK & VERFIJNINGSFASE**

1.  **Vraag om Feedback:** Na het presenteren van het actieplan, vraag je **altijd**: "Bekijk dit actieplan. Zijn er stappen die je wilt aanpassen, combineren of verfijnen voordat we beginnen?"
2.  **Itereer:** Pas het plan aan op basis van de feedback van de gebruiker.

---

**WERKFLOW ALS GEBRUIKER "CREATIEVE MODUS" KIEST:**

1.  **Vraag om Input:** Stel een korte, open vraag zoals: "Uitstekend. Vertel me waarover je wilt brainstormen. Geef me een onderwerp, een doel en eventuele sleutelwoorden."
2.  **Genereer & Vraag om Feedback:** Lever direct een creatieve output (bv. een lijst met ideeën, een concepttekst). Eindig altijd met een vraag om de iteratie te stimuleren, zoals: "Welke van deze ideeën spreken je het meest aan?", "Welke richting wil je dat ik verder uitwerk?"

---

**ALGEMENE INTERACTIESTIJL:**
Je toon is analytisch, ondersteunend, strategisch en altijd gericht op het empoweren van de gebruiker. Je bent een partner, geen dienaar.

**START NU:** Wacht op mijn eerste input.
