# TRES AI-agency dashboard

Het dashboard staat in `tres-dashboard/index.html`: één gebouwd bestand (~85 KB) met HTML, CSS, JS en alle data.
Openbare versie: https://ai-agency-voor-tres.vercel.app (Denzel deployt zelf via Vercel).

**Lees het bestand nooit helemaal.** Zoek met grep op een kopje of veldnaam en lees alleen dat stukje.

Opbouw:
- Regel 25 begint de script: data staat in `const k=…,w=…,…,c=[…]` (eindigt vóór `,h=e=>`); daarna volgen per hoofdstuk sjabloonfuncties.
- Hoofdstukken (`<section class="hoofdstuk" id="…">`, volgorde in `c`): einddoel (S), werking (architectuur-stack staat hardcoded in functie R + T, k, w), agents (C), linkedin (functie Q, data inline), werkwijzen ($), data (y), veiligheid (I), keuze (v: advies, vertaling, onderdelen met kostenClaude/kostenChatgpt, checken, bronnen), modellen (d), bouwen (f: fases met stappen), naslag (A, m, z, E).
- Architectuur: Jij → AI Marketing Director (platform nog open: Claude of ChatGPT) → Growth-agents BE en DE → 6 gedeelde specialisten → koppelingen (Windsor.ai, MailBlue, Leadinfo & Forms, Zapier & CRM) → kwaliteitscontrole & goedkeuring.
- Eerste toepassing: LinkedIn-reactievoorstellen bij posts van anderen; AI plaatst nooit zelf.

Na een aanpassing: render met Playwright (check JS-fouten en 400px-breedte), stuur Denzel het bestand, en commit + push alleen als hij dat vraagt.
