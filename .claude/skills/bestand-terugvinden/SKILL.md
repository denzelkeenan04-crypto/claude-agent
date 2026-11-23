---
name: bestand-terugvinden
description: Vaste zoekroute om een kwijtgeraakt bestand echt te vinden in plaats van de gebruiker te vragen waar het staat. Gebruik bij "waar is mijn ...", "ik kan ... niet vinden", "waar staat dat bestand van gisteren".
---

# Bestand terugvinden

## Doel
Het bestand gevonden, met een pad waar je op kunt klikken. Of een eerlijk "niet gevonden", met waar je gezocht hebt.

## Stappen
1. **Zoeken op naam.** Zoek op een woord uit de naam in de eigen mappen van de gebruiker (op een Mac met `mdfind`/Spotlight, anders `find`/Glob). Sla systeemmappen, caches en `node_modules` over. Weet de gebruiker de naam niet, zoek dan op een woord dat ín het bestand staat (Grep). Kan een naam twee dingen zijn (bijv. de opdracht én het ingeleverde werk), noem dan beide.
2. **Opruimlijsten.** Is er een opruimmap met verplaats-lijsten (zoals `manifest.json`), zoek daar ook in en zeg wat er verplaatst is en waarheen.
3. **Recent gewijzigd.** Weet de gebruiker alleen ongeveer wanneer, kijk dan naar bestanden die in die dagen zijn veranderd.
4. **Kiezen.** Meerdere versies? Zet ze onder elkaar met datum en zeg welke de nieuwste is. Sla tijdelijke bestanden over (zoals Word-bestanden die met `~$` beginnen).
5. **Uitslag.** Gevonden: het pad. Niet gevonden: waar je zocht, en waar de gebruiker zelf nog kan kijken (Prullenmand, iCloud, Google Drive).

## Voorbeeld van een goede uitslag
> Gevonden, 3 versies van je verslag:
> - `Downloads/Inleveren/verslag-v3.docx` (nieuwste, 20-11)
> - `Downloads/verslag-v2.docx` (18-11)
> - `Documenten/verslag.docx` (12-11)
>
> Zal ik de nieuwste openen?

## Grenzen
Niet verwijderen, niet overschrijven, niets uit de Prullenmand halen. Verplaatsen of hernoemen alleen als de gebruiker erom vraagt, en zeg dan precies wat waarheen ging.
