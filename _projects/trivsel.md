---
layout: default
title: "Håndtering af ordinal data i trivselsundersøgelser"
image: "/assets/projects/kidsname-thumbnail.png"
mathjax: true
layout: post
excerpt: "How to analyze well-being surveys. Article in Danish."
date: 2025-09-26
---

En trivselsundersøgelse gentages med ét års mellemrum på en arbejdsplads med *N* ansatte. Formålet er at undersøge trivslen blandt de nuværende ansatte. Resultatet for hvert år angives som et gennemsnit (af respondenterne) og kan ligge mellem 1 og 5.

Lad *x₁* være det målte gennemsnit af respondenterne i år 1. Lad *n₁* være antallet af respondenter i år 1 (maksimalt *N*). Lad *x₂*, *n₂* være tilsvarende for år 2. Lad nu *y₁* og *y₂* være hhv. den gennemsnitlige trivselsscore i år 1 og år 2 for hele arbejdspladsen. Bemærk at disse er uobserveret da ikke alle har svaret.

Lad os definere Δ*x* = *x₂* - *x₁*. Dette er den observerede forskel (blandt respondenterne) fra år 1 til år 2. Definer også Δ*y* = *y₂* - *y₁* som er den faktiske forskel fra år 1 til år 2 for hele arbejdspladsen. Bemærk at vores bedste bud på sidstnævnte forskel -- et bud som vi betegner Δ̂*y* -- er den målte forskel fra trivselsanalysen:

$$\widehat{\Delta y} = \Delta x \quad (1)$$

En nedre grænse for forskellen Δ̂*y*₍ₙₑ𝒹ᵣₑ₎ kan findes ved at forestille sig, at de ansatte der ikke besvarede undersøgelsen i år 2 (*N* - *n₂*) ville svare så **lavt** så muligt (dvs. en score på 1), samtidig med at ansatte der ikke besvarede undersøgelsen i år 1 (*N* - *n₁*) ville svare så **højt** som muligt (dvs. en score på 5). Formelt:

$$\widehat{\Delta y}_{\text{nedre}} = \frac{x_2 n_2 + (N-n_2) - (x_1 n_1 + 5(N - n_1))}{N} \quad (2)$$

Tilsvarende kan vi finde en øvre grænse for forskellen Δ̂*y*₍øᵥᵣₑ₎ ved at forestille sig, at de ansatte der ikke besvarede undersøgelsen i år 2 (*N* - *n₂*) ville svare så **højt** så muligt (dvs. en score på 5), samtidig med at ansatte der ikke besvarede undersøgelsen i år 1 (*N* - *n₁*) ville svare så **lavt** som muligt (dvs. en score på 1). Formelt:

$$\widehat{\Delta y}_{\text{øvre}} = \frac{x_2 n_2 + 5(N-n_2) - (x_1 n_1 + (N - n_1))}{N} \quad (3)$$

## Eksempel

**Eksempel:** Vi undersøger en arbejdsplads med *N* = 10 ansatte. Første år svarede *n₁* = 9 respondenter. Andet år svarede *n₂* = 8 respondenter. De årlige gennemsnit var *x₁* = 4.1 og *x₂* = 3.8. Vores bud på arbejdspladsens forskel i trivsel er Δ̂*y* = 3.8 - 4.1 = -0.3.

Eksakt øvre og nedre grænse er:

$$\widehat{\Delta y}_{\text{nedre}} = \frac{3.8 \times 8 + (10 - 8) - (4.1 \times 9 + 5 \times (10 - 9))}{10} = -0.95 \quad (4)$$

$$\widehat{\Delta y}_{\text{øvre}} = \frac{3.8 \times 8 + 5 \times (10 - 8) - (4.1 \times 9 + (10 - 9))}{10} = 0.25 \quad (5)$$
