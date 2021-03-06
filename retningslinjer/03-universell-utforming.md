---
layout: page
group: guidelines
permalink: /guidelines/uu.html
title: Universell utforming
description: Retningslinjer
---

<div id="alert-no-arrow" class="a-message a-message-error a-message--arrow-off a-message--fullwidth mb-2 a-py-minus-1">
  NB: Innholdet og sidene er under utvikling
</div>

## Tilgjengelighet

Det er viktig gjøre innhold tilgjengelig for alle. God tilgjengelighet kan hjelpe mennesker med funksjonshemninger å oppfatte innholdet vårt på en meningsfull måte. Dette gjelder f.eks blindhet, nedsatt syn og hørsel, lærevansker og begrenset bevegelse. Det er flere ting vi kan gjøre, men det første og viktigste er å skrive semantisk god HTML.

Forskrift om universell utforming av IKT-løsninger stiller krav om at nettsider må oppfylle 35 av 61 suksesskriterier i standarden [Retningslinjer for tilgjengelig webinnhold (WCAG) 2.0](https://www.w3.org/Translations/WCAG20-no/). Sjekk ut [minimumskravene](https://uu.difi.no/krav-og-regelverk/wcag-20-standarden/) på difi som er omfattet av forskriften.

## Mål for universell utforming (UU)

- Løsningen skal fungere 100% ved tab-navigering, med logisk og meningsfull fokusrekkefølge.  Tab-indeks må vurderes. Det elementet som er i fokus skal få en egen stilsetting, slik at det er tydelig hvor man står.
- For å sørge for en god brukeropplevelse for blinde, skal sidemalene testes i skjermopplesere. Det er viktig at man er bevisst på om det blir brukt knapper eller linker, da skjermlesere kan få problemer med å tolke funksjonaliteten.
- alt- og title-attributter skal brukes til å gi tilleggsinformasjon til bilder og andre objekter.
- label-element skal ha et for-attributt som matcher skjemakontrollen det tilhører, med mindre label omslutter input-feltet.
- Ulike typer lenker skal brukes riktig (disse har ulikt design basert på om de står sammen med annen tekst, eller om de lenker til interne/eksterne sider)
- Alle sidemaler skal tåle tekststørrelsesendring på opptil 200% uten å brekke eller at tekst forsvinner.
- Alle klikkbare elementer skal være minimum 48px på korteste side. Elementer trenger ikke oppfylle dette visuelt, men kan få et usynlig touch-område rundt seg.

Dynamisk innhold er alltid litt vanskelig med tanke på UU, bruk aria-tags.

[Tilpasse WCAG 2.0 sjekkliste for prosjekt](https://www.w3.org/WAI/WCAG20/quickref/) (offisiell)

WCAG-krav er retningslinjer, ikke krav. Dersom avvik skjer, bør det finnes en god begrunnelse for avviket.

## Rutiner
For å sikre best mulig kvalitet på løsningen, bruk følgende verktøy/steg:

1. Sjekk Errors og Alerts i [Wave Toolbar](http://wave.webaim.org/extension/)
2. HTML skal validere (som [HTML5](https://html5.validator.nu/)).
3. Test skjermleserfunksjonalitet (Overskrift-hopping, tabbing, lenker og vanlig lesing)
 med [ChromeVox](https://chrome.google.com/webstore/detail/chromevox/kgejglhpjiefppelpmljglcjbhoiplfn).
3. Skru av CSS i nettleseren og sjekk at rekkefølge på komponenter er logisk.
4. Kjør [Accessibility Developer Tools](https://chrome.google.com/webstore/detail/accessibility-developer-t/fpkknkljclfencbdbgkenhalefipecmb) Audits fane i dev tools.


Disse stegene er blitt tatt som standard design-review. I tillegg bør det testes på **ekte brukere** der det er mulig.

Andre nyttige verktøy som kan tas i bruk dersom man trenger mer utdypende info er:

- Kjør Ainspector Sidebar i Firefox (denne deler opp evt feil inn i WCAG standards)
- NoCoffee simulator viser hvordan brukere med nedsatt syn opplever nettsiden
- ChromeLens (legges på i dev tools) kan brukes til å simulere nedsatt syn
