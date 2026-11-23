---
name: rapportage-agent
description: Bouw een agent of automatisering die op een vaste dag cijfers ophaalt, er per doelgroep (medewerker, manager, directie) een rapport van schrijft en het als concept klaarzet. Gebruik bij "rapport op vaste dag", "weekrapport", "maandrapport automatiseren".
---

# Rapportage-agent per doelgroep

## Idee: één agent, één workflow per doelgroep
| Voor wie | Hoe vaak | Inhoud |
|---|---|---|
| Elke medewerker apart | Wekelijks (bijv. ma 7:00) | Alleen zijn **eigen** openstaande zaken en totaal |
| Manager | Wekelijks | Eén samenvatting per medewerker |
| Directie | Per kwartaal | Grote lijnen: verloop per maand, omzet per bron |

## Stappen
1. **Data klaarzetten** in één bron (Sheets, Airtable, HubSpot, database) met duidelijke tabellen en een kolom die zegt of iets open staat.
2. **Kies het gereedschap:** GitHub Actions + Claude, n8n, Make of Relay.app. Koppel databron + mail/Slack.
3. **Per doelgroep één workflow** met een korte opdracht: wanneer, uit welke tabel, voor wie, wat erin moet.
4. **Rekenen gebeurt in code, niet door de AI.** Een script haalt de cijfers op, vergelijkt met de vorige periode en rekent verschillen uit. De AI schrijft alleen 3–5 zinnen uitleg.
5. **Controle:** een script checkt dat elk getal in de tekst echt in de cijfers staat. Ontbreekt een cijfer, dan staat dat in het rapport. De AI verzint geen oorzaak of advies.
6. **Testen naar het eigen adres** van de gebruiker; lees het rapport na. Pas de instructie aan als er iets niet klopt (bijv. een code i.p.v. een naam).
7. Herhaal voor manager en directie.

## Grenzen
- Versturen naar echte mensen pas na "ja" van de gebruiker; tot die tijd is alles een concept.
- Privacy: elke medewerker ziet alleen zijn eigen cijfers.
- Een kwartaalrapport testen vóór het kwartaal om is geeft lege uitkomsten; dat is normaal.
- Geen tokens of wachtwoorden in bestanden; gebruik secrets.
