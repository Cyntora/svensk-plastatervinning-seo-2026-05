# Designregler och tonregler för denna leverans

Reglerna som styrde produktionen av rapporten. Bevarade här så att kommande versioner och liknande leveranser följer samma standard.

## Design

- Single-file HTML med inbäddad CSS. Ingen build-process.
- Matcha kundens brand. Kolla deras hemsida för färger, typografi och känsla.
- Cyntoras logotyp (SVG inline) i nav och hero. Hämtad från cyntora.se.
- **Favikon krävs.** Lägg `favicon.svg` (Cyntoras C-mark) bredvid `index.html` och länka i `<head>` via `<link rel="icon" type="image/svg+xml" href="favicon.svg">`. Skapas genom att ta de två första path-elementen från Cyntora-loggans SVG och sätta `viewBox="0 0 71 71"`.
- Cormorant Garamond för rubriker, Inter för brödtext.
- Scroll-deck-format. Varje sektion fyller sin egen vy.
- 16:9 PDF (1600x900) som backup utöver HTML.

## Färgpalett, denna kund

Varma, naturnära toner som matchar kundens hållbarhetsprofil:

- Bakgrund: `#F6F1E8` (varm cream)
- Bakgrund alt: `#EFE8DA`
- Paper: `#FBF7F0`
- Bläck: `#1B1B1F`
- Bläck mjuk: `#4A4A52`
- Linje: `#E1D9C8`
- Sage (accent): `#6F8472`
- Sage mjuk: `#B7C2B0`
- Varm (accent): `#C68C6E`
- Varm mjuk: `#E8C9B6`
- Good: `#5A7A55`
- Warn: `#B45A3C`

## Tonregler

Detta är de viktigaste reglerna. Brott mot dem ska åtgärdas innan publicering.

- Skriv som Filip skriver i Gmail och Slack: direkt, korta meningar, "ni"-form i offerter. Cyntoras egen offerttext är referens.
- INGA tankstreck (—). Använd komma, punkt eller "och" istället.
- INGA AI-marknadsförarklichéer. Exempel som ska undvikas:
  - "lågt hängande frukter"
  - "B2B-guld"
  - "edge inte svaghet"
  - "snabba vinster och långsiktig pipeline"
  - "italiensk kvalitet möter svensk ambition"
  - "vi bryr oss med hjärna med hjärta"
- INGA fauxpoetiska rubriker med italics-emfas. Rubriker beskriver vad sektionen handlar om.
- Inga triadiska konstruktioner för effekt.
- Citatcitering av sidtitlar och liknande får använda kursiv stil eller citationstecken, men inte för att skapa stämning.

## Publicering

- Publikt GitHub-repo via gh CLI under Cyntora-organisationen.
- Pusha index.html, slides.pdf, README.md, RULES.md.
- Aktivera GitHub Pages på main-branch.
- `<meta name="robots" content="noindex, nofollow">` så Google inte indexerar kundens prisuppgifter eller siffror.
- Returnera live-URL till Filip när det är live.

## Leverans

- HTML-fil lokalt
- favicon.svg
- 16:9 PDF (1600x900) som backup
- Live URL på github.io
- Förslag på kort mejl till kunden med länken
- README.md med översikt
- RULES.md med dessa regler
