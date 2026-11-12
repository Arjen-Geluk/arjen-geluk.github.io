# Arjen's GitHub — conventies

Dit is de overkoepelende portfoliosite (GitHub user page) van Arjen Geluk,
en het leidende document voor de structuur van al zijn repo's.

## Structuur

- `arjen-geluk.github.io` (deze repo) is de speciale GitHub user-page repo:
  wordt automatisch gepubliceerd op de root `https://arjen-geluk.github.io/`.
  Bevat alleen de landingspagina met rubrieken (`index.html`) die doorlinkt
  naar de losse topic-repo's.
- Elk onderwerp krijgt een eigen repo (geen submappen voor losse onderwerpen
  in deze repo). Binnen een topic-repo staat elk los project/deliverable in
  een eigen submap met zijn eigen `index.html`.
- Huidige topic-repo's:
  - [Navigation](https://github.com/Arjen-Geluk/Navigation) — zeilen &
    navigatie: vaargebieden, getijkaart, wedstrijdberekeningen.
  - Nog te maken: brommer-reizen, techniek & industrie, software & scripts.

## Rubrieken op de landingspagina

Vast houden aan deze vier categorieën (sectie-titels in `index.html`):
Zeilen & navigatie, Brommer-reizen, Techniek & industrie, Software & scripts.
Elke categorie is een `<section class="paneel">` met een `h2`. Een categorie
zonder projecten krijgt een `<div class="leeg">` i.p.v. een kaart. Zodra een
topic-repo een werkende GitHub Pages-site heeft, komt er een `<a class="kaart">`
met link naar die site.

## Licentie

Alle repo's in dit portfolio gebruiken CC BY-NC-ND 4.0 (zie `LICENSE` in
elke repo): bekijken en gebruiken mag, hergebruik/aanpassen/commercieel
inzetten niet zonder toestemming. Geen losse licentiekeuzes per repo zonder
overleg.

## Naamgeving & publiceren

- Repo-namen in het Engels, kleine letters waar mogelijk (GitHub Pages-URL's
  zijn toch lowercase).
- GitHub Pages: altijd "Deploy from a branch", branch `main`, map `/ (root)`.
- Nieuwe repo's aanmaken kan niet automatisch vanuit een Claude Code sessie
  (sessie is gebonden aan al gekoppelde repo's) — Arjen maakt een lege repo
  zelf aan via github.com/new (Public, README aanvinken, license op "None"),
  waarna de repo aan de sessie gekoppeld kan worden.
- Permanent verwijderen van een repo doet Arjen altijd zelf (Settings →
  Danger Zone); dat voert Claude nooit automatisch uit.

## Huisstijl (design system Navigation)

Alle pagina's in alle repo's volgen één huisstijl: het design system **Navigation**,
https://claude.ai/artifact/6F27EjgQKsX2xBuRW7kX1i. Lees daar eerst `project/README.md`
(Artifact-tool, `read` met `path`), en voor waarden `project/tokens.json` en
`project/components/bundle.css`.

- Tokens (`bg`, `panel`, `ink`, `muted`, `line`, `navy`, `accent`, …) in een licht en een donker thema;
  donker volgt `prefers-color-scheme`. Componenten: Kopbalk, Paneel, Knop, Chip, Melding, Veld,
  Lijsttabel, Polartabel.
- Landingspagina's (deze en die van elke topic-repo): navy kopbalk met ankerring en de naam in
  hoofdletters, daaronder panelen met kaarten. `index.html` in deze repo en in Navigation zijn het
  voorbeeld. Nederlandstalige teksten.
- Elke pagina heeft in de kopbalk een terugknop (`<a class="terug">`) naar de pagina één niveau
  hoger: een project naar de landingspagina van zijn topic-repo (`href="../"`), een topic-landingspagina
  naar deze portfoliosite (`https://arjen-geluk.github.io/`, "← Arjen Geluk"). Alleen deze
  portfoliopagina zelf heeft er geen.
- Waarden worden inline in de pagina gezet, niet geladen uit het design system.
- Een nieuwe topic-repo krijgt in zijn `CLAUDE.md` een sectie "Huisstijl (design system)" met deze
  link en afspraken (zie `CLAUDE.md` van Navigation), en zet zijn landingspagina eerst in de huisstijl.
- Komt er een nieuwe kleur of een nieuw component bij: werk dan ook het design system bij.

## Favicon

De favicon-set (poolster) staat in de root van deze repo en is daarmee voor het hele domein
`arjen-geluk.github.io` beschikbaar: `favicon.ico`, `favicon.svg`, `apple-touch-icon.png`,
`icon-192.png`, `icon-512.png`, `site.webmanifest` (naam "Arjen Geluk"). Elke pagina in elke
repo zet in de `<head>`:

```html
<link rel="icon" href="/favicon.ico" sizes="32x32">
<link rel="icon" href="/favicon.svg" type="image/svg+xml">
<link rel="apple-touch-icon" href="/apple-touch-icon.png">
<link rel="manifest" href="/site.webmanifest">
<meta name="theme-color" content="#12263F">
```

Topic-repo's met de afspraak "alles inline" zetten daarnaast het SVG-icoon als data-URI in de pagina.
