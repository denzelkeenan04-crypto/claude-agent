---
name: zuinig-met-tokens
description: Tips en vaste gewoontes om minder tokens te verbruiken en minder snel tegen de Claude-limiet aan te lopen (kleine CLAUDE.md, cache niet breken, juiste model per klus, korte chats). Gebruik bij "mijn limiet is op", "hoeveel tokens", "hoe kan het zuiniger", of bij het opschonen van CLAUDE.md en skills.
---

# Zuinig met tokens

Bronnen: video's van Duncan Rogoff, Nate Herk en Miles Deutscher (geleerd nov. 2026). Getallen komen uit de video's en kunnen veranderen; controleer bij Anthropic als het ertoe doet.

## 1. Minder inlezen bij het opstarten
- **CLAUDE.md klein houden, als een kaart.** Alleen waar welk bestand staat en de vaste regels. De rest in losse bestanden, één onderwerp per bestand (schrijfstijl, huisstijl, doelgroep, aanbod).
- **Elk feit op één plek**, verwijs ernaar. Kopieën raken verouderd.
- **Bovenaan elke skill: wanneer hij gebruikt moet worden.** Een skill is een map met `SKILL.md`; na het maken een nieuwe sessie starten.
- **Vaste route in de skill zetten** (bijv. "gebruik yt-dlp"), dan hoeft Claude niet te gokken.
- Ging iets eindelijk goed? Maak er meteen een skill van.

## 2. De cache niet breken
Wat Claude al gelezen heeft, wordt even onthouden en kost dan ongeveer een tiende.
- Abonnement in Claude Code: ±1 uur. API, sub-agents en "extra usage": ±5 minuten.
- **Chat > 1 uur stil?** Begin liever opnieuw met een overdracht.
- **Nieuw onderwerp = nieuwe chat** (`/clear`).
- **Overdracht i.p.v. `/compact`:** laat een samenvatting maken (gedaan, bestanden, open punten, waar verder), `/clear`, plak hem terug.
- **Niet van model wisselen midden in een chat**; elk model heeft een eigen cache. "Opus plan" wisselt ook.
- CLAUDE.md aanpassen midden in een chat mag; het werkt pas na herstart.

## 3. Slimmer werken
- **Praten is goedkoop, bouwen is duur.** Eerst plannen ("maak eerst een plan"), dan bouwen.
- **Juiste model per klus:** Opus voor moeilijk werk en beslissingen, Sonnet voor het meeste werk, Haiku voor snelle klusjes (gegevens uitlezen).
- **Inspanning lager** (medium/laag) voor simpel werk.
- **"Wees beknopt"** in de vaste instructies.
- **Grote klus in stukken**, controleren na elk stuk.
- Eerst optimaliseren, dan pas upgraden. Gebruik bekijken: claude.ai/settings/usage.

## Grenzen
CLAUDE.md of skills inkorten alleen na "ja" van de gebruiker en met eerst een kopie. Vaste veiligheidsregels (niets verwijderen, niets versturen zonder "ja", geen wachtwoorden) blijven altijd in CLAUDE.md staan.
