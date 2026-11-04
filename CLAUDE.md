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
Een categorie zonder projecten krijgt een `<div class="placeholder">` i.p.v.
een kaart. Zodra een topic-repo een werkende GitHub Pages-site heeft, komt
er een `<a class="card">` met link naar die site.

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

## Stijl landingspagina's

Donker thema, minimalistische kaarten-grid (zie `index.html` in deze repo
en in Navigation als voorbeeld), Nederlandstalige teksten.
