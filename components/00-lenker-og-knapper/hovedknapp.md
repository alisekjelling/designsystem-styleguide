---
layout: component-detail
group: komponenter
subgroup: lenker-og-knapper
permalink: /komponenter/lenker-og-knapper/knapp.html

title: Knapp
description:


variations:
- title: Knapp
  description: Brukes for handlinger, f.eks Lagre, Send, osv. Siden knappen er kun 36px høy, er det avsatt et område over og under, slik at touch target er 48px. Det skal være minimum 12px mellomrom mellom hver knapp/lenke.
  styleModifier: a-btn
  includeClassification: atoms
  includeCategory: 03-knapper
  includeName: 10-knapp
- title: Knapp fare
  description: Rød knapp brukes for å advare brukeren mot handlingen. F.eks. Slett, Avbryt, osv.
  styleModifier: a-btn-danger
  includeClassification: atoms
  includeCategory: 03-knapper
  includeName: 12-knapp-fare
- title: Knapp Suksess
  description: Grønn knapp brukes for
  styleModifier: a-btn-success
  includeClassification: atoms
  includeCategory: 03-knapper
  includeName: 11-knapp-suksess

  usage:
  - title: When to use
    description: Usage description.
  - title: When to consider an alternative
    description: Alternative usage.

  classes:
  - className: c-hero
    required : yes
    description: Apply to the hero block's containing HTML element. This class sets up the background-image handling and text color for the unit. The `c-hero` element should have just one immediate child, the `c-hero__body` element. Note, too, that the unit's hero image should be applied as a background image to this `c-hero` element.
  - className: c-hero--bare
    modifier : yes
    description: Add to the `c-hero` element to remove the default gradient overlay from the hero image.
  - className: c-hero--tinted
    modifier : yes
    description: Add to the `c-hero` element to replace the default gradient overlay with a solid, uniform tint.
  - className: c-hero__body
    required: yes
    description: Apply to the container for the card body, which typically includes a title and description (see below) but can include any arbitrary markup including buttons for a call to action. The class manages the card's background gradient.
  - className: c-hero__title
    recommended: yes
    description: Apply to the card's heading inside the card body. The recommended element for this class is `<h1>`.
  - className: c-hero__desc
    recommended: yes
    description: Apply to the card's description text inside the card body. The recommended element for this class is `<p>`.

---
