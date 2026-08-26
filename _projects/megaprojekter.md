---
title: "Megaprojekter"
image: "/assets/projects/megaprojekter-thumbnail-2.png"
mathjax: true
layout: post
excerpt: "Store danske IT- og anlægsprojekter har været ramt af forsinkelser og fordyrelser. Her undersøger jeg tallene."
date: 2026-08-26
lang: da
---

<style>
.fig-bred {margin: 1.5em 0; text-align:center; }
.fig-bred img { max-width: 100%; height: auto; }
/* Ved under 280 px vises mobiludgaven */
@media (max-width: 820px) {
  .fig-bred img{ max-width: min(100%, 460px); }
}
/* Uden sidebar */
@media (min-width: 821px) and (max-width: 69.99em) {
  .fig-bred.udbrud { width: min(1200px, calc(100vw - 4em));
                     margin-left: 50%; transform: translateX(-50%); }
}
/* Med sidebar */
@media (min-width: 70em) {
  .fig-bred.udbrud { width: min(1200px, calc(100vw - 21em));
                     margin-left: 50%; transform:translateX(-50%); }
}
</style>

> Over budget, over time, under benefit. Over and over again.
>
> — Bent Flyvbjerg, Professor Emeritus

Citatet indrammer det som Bent Flyvbjerg - ekspert i Project Management - har kaldt  **Jernloven for megaprojekter**. I følge Bent Flyvbjerg overskrider langt størstedelen af projekter deres budget- og tidsramme, og bliver af ringe kvalitet.

I bogen **How To Get Big Things Done** går Bent Flyvbjerg og Dan Gardner i dybden med de psykologiske og beslutningsmæssige problemer der driver denne såkaldte lov inden for projektplanlægning.

Inspireret af bogen satte jeg mig for at efterprøve Jernloven på en række danske megaprojekter.


<figure style="text-align: center;">
 <img src="/assets/projects/how_to_get_big_things_done.png" alt="Bog om megaprojekter af Bent Flyvbjerg" width="400">
 <figcaption style="text-align: center;">
   Bogens forfattere beskriver hvorfor (mega)projekter sjældent forløber gnidningsfrit.
 </figcaption>
</figure>

## Datagrundlaget: megaprojekterne

Jeg gik på jagt online efter store, velbeskrevne danske projekter. Som udgangspunkt har medierne ikke interesse i at beskrive megaprojekter, medmindre der er forhold at kritisere, som når budgetrammen sprænges. Den helt store undtagelse er tiden omkring projektets tilblivelse, i det megaprojekter som supersygehuse og broer trods alt er af samfundsmæssig interesse.

Min søgning tog udgangspunkt i projekter, jeg på forhånd havde et vist kendskab til. Da kendskab typisk hænger sammen med omtale, og omtale formodes at hænge sammen med kritisable forhold, vil mit udvalg af projekter naturligvis være biased mod dem der udviser mangler.

Mit datagrundlag omfatter imidlertid de største og mest omtalte projekter på dansk jord med milliardindsprøjtninger. Selv hvis de ikke er repræsentative for projekter af mindre størrelsesorden, er forsinkelser og fordyrelser i netop disse megaprojekter af betydelig samfundsmæssig interesse.

For hvert projekt forsøgte jeg at identificere det oprindelige og endelige budget samt den oprindelige og senest kendte deadline i kalender år. Hvis der ikke fandtes en troværdig kilde til budgettet, registrerede jeg det ikke. Samme princip gjaldt for projektets deadline.

Priserne blev reguleret efter [økonomistyrelsens prisindeks](https://oes.dk/statsregnskab/finanslov-og-udgiftsopfoelgning/indeks/regulering-af-anlaegsprojekter/) og angivet i 2025 priser.

## Over budget, over time - under benefit?

Resultatet af undersøgelsen, som omfattede 18 IT- og anlægsprojekter, viste konsekvente overskridelser i både budget og tid (Se Figur nedenfor). Den eneste undtagelse var Det Nye Universitetshospital Aarhus (DNU) der efter kilderne at dømme blev færdig planmæssigt. 

Ét projekt skiller sig særligt ud, og det er ejendomsvurderingssystemet (ICE), der præsterede at gå fra et startbudget på 116 millionar og til 4.9 milliarder, svarende til en procentvis overskridelse på ca. 4124%. Tilmed blev ejendomsvurderingssystemet forsinket med hele 8 år, fra 2017 til 2025.

Af andre betydelige fordyrelser og forsinkelser finder man Niels Bohr bygningen med et budgetoverskridelse på 149% og 8 års forsinkelse samt Nyt Hospital Nordsjælland med en foreløbiog overskridelse på 103% og forsinkelse på 7 år.

Medianen for den procentvise overskridelse af et projekts budget ligger på 39%, mens medianen for et projekts forsinkelse ligger på 5 år.

Hvorvidt de færdige projekter indfrier forventningerne, er svært at fastslå entydigt. For ejendomsvurderingssystemet er der dog ingen tvivl. Adskillige fejl og astronomiske ejendomsvurderinger har gjort det aldeles upopulært blandt borgere og givet grå hår i Vurderingsstyrelsen. Trods forsinkelser og milliardoverskridelser kan projektet altså ikke siges at have indfriet de målsætninger, der blev opstillet. For de andre færdige projekter er det endnu for tidligt at afgøre. Dog er der indikationer på, at passagertallet i Hovedstadens Letbane er langt under det niveau, der var anslået forud for projektets start.

<figure class="fig-bred udbrud">
  <picture>
    <source media="(max-width: 820px)" srcset="/assets/projects/jernloven_danske_projekter_mobil.png">
    <img src="/assets/projects/jernloven_danske_projekter.png"
         alt="Budget- og tidsoverskridelser for en række danske megaprojekter">
  </picture>
</figure>

Tallene skal tages med en række forbehold:

* **Kildeafvigelser:** I nogle tilfælde findes der kilder der er uenige om de oprindelige budgetter, prisindeks samt hvad rammen præcis dækker. Kun de mest troværdige og detaljerede kilder er anvendt, og projekter med stor diskrepans er sorteret fra.
* **Forskellige baselines:** Det allokerede budget varierer alt efter, om der tages udgangspunkt i den første politiske aftale, anlægsloven eller kontraktindgåelsen. Korrektionsreserven (den budgetmæssige buffer) er størst tidligt og falder, efterhånden som projektet tager form. Det kan få enkelte projekter til at fremstå uforholdsmæssigt dyre tidligt i forløbet.
* **Regnskabsmæssige og projektmæssige tilpasninger:** Tallene kan påvirkes, hvis projektdele skrottes for at overholde budgettet, eller hvis omkostninger bogføres uden om anlægsrammen. Eksempler er Aarhus' nye fodboldstadion, hvor man skar pladser væk for at undgå budgetoverskridelser, Banedanmark, der bogførte en ekstraomkostning på 2,2 mia. kr. til Signalsystemet som drift, samt DNU, hvor en engangsudgift på 1 mia. kr. blev holdt uden for anlægsrammen.
* **Etapevis ibrugtagning:** Flere projekter forløber i etaper/faser. I sådanne tilfælde benyttes det samlede projekts afslutningsår som målestok.

## Den sorte svane

Nobelprismodtageren og psykologen Daniel Kahnemann blev blandt andet kendt for sin bog **Thinking, Fast and Slow** hvori han beskriver system 1 hjernen (den hurtige tænkning) og system 2 hjernen (den langsomme tænkning). Når opgaver er komplekse er det nødvendigt at vi aktiverer system 2.

I bogen **How To Get Big Things Done** bliver læseren introduceret til mantraet 'Think Slow, Act Fast' med henvisning til Kahnemanns system 2. Idéen er at megaprojekter er komplekse og kræver omhyggelig planlægning. Det siger næsten sig selv. Men i en verden, hvor tid er penge, har langsom tænkning ikke høj salgsværdi hos ejerkredsen. For jo hurtigere vi kommer i gang, desto hurtigere er vi færdige.

Det er også en besnærende tanke, som dog overser, at når vi først er igang, er risikoen størst. Flyvbjerg og Gardner beskriver det som et vindue der står åbent. Mens projektet pågår, kan der ryge alverdens ting ind og forstyrre projektet, herunder en sort svane.

Den sorte svane er billedet på noget yderst sjældent. Det kan være en pandemi eller en recession, som påvirker projektets tidshorisont og økonomi. Det siger sig selv, at jo længere et vindue (projektet) er åbent, desto større er risikoen for at en sort svane flyver ind. 

Det samme princip kan formuleres statistisk. De fleste er bekendt med begrebet *regression to the mean* der fortæller at når du oplever noget usædvanligt, skal du ikke regne med at det bliver ved: det hverdagslige er normalen. Men det omvendte gælder også. Selvom dine dage ligner hinanden, så kan du godt regne med at før eller siden så sker det usædvanlige. Det kalder vi *regression to the tail*. Med tail, menes yderligheden i en sandsynlighedsfordeling. Det er her den sorte svane holder til.

<figure class ="fig-bred">
  <picture>
    <source media="(max-width: 820px)" srcset="/assets/projects/think_slow_act_fast_mobil.png">
    <img src="/assets/projects/think_slow_act_fast.png"
         alt="Plot med to scenarier der viser at god planlægning er bedre end hurtig eksekvering">
  </picture>
</figure>

## Referencer

### Cityringen (Metro)

-   <https://www.kk.dk/sites/default/files/agenda/3e5364cf-41d1-4b2f-bac8-a83b3ccb3e96/39095bf2-2af3-4936-8561-7af56cee1efd-bilag-2.pdf>
-   <https://ing.dk/artikel/efter-otte-aars-arbejde-ni-maaneders-forsinkelser-koebenhavns-cityring-aabner-29-september>

### Nyt Aalborg Universitetshospital

-   <https://byghospitalsbyen.rn.dk/Anlaegsprojekter/Nyt-Aalborg-Universitetshospital/Om-Nyt-Aalborg-Universitetshospital>
-   <https://sundhedspolitisktidsskrift.dk/nyheder/sundhedspolitik/11141-fra-gyserrapporter-og-milliardoverskridelser-til-patienter-i-sengene-nyt-hospital-i-aalborg-taget-i-brug.html>
-   <https://www.ft.dk/samling/20222/almdel/fiu/bilag/54/2658783.pdf>

### Nyt Hospital Nordsjælland

-   <https://www.rigsrevisionen.dk/revisionssager-arkiv/2023/nov/beretning-om-byggeriet-af-nyt-hospital-nordsjaelland>
-   <https://www.dr.dk/nyheder/indland/nordsjaellandsk-hospital-bliver-dobbelt-saa-dyrt-en-skandale>
-   <https://www.sn.dk/art6554222/hilleroed-kommune/nyhed/voldsom-stigning-nu-bliver-supersygehus-i-nordsjaelland-dobbelt-saa-dyrt/>

### Nyt Odense Universitetshospital

-   <https://ft.dk/samling/20222/almdel/fiu/bilag/54/2658783.pdf>
-   <https://nyheder.tv2.dk/samfund/2024-11-25-nyt-supersygehus-i-odense-bliver-endnu-en-gang-forsinket-og-dyrere>

### Det Nye Universitetshospital Aarhus (DNU)

-   <https://www.rm.dk/siteassets/om-os/aktuelt/2017/februar-17/rigsrevision/fakta-om-byggeriet-af-dnv-skejby-aarhus.pdf>
-   <https://www.ft.dk/samling/20222/almdel/fiu/bilag/54/2658783.pdf>
-   <https://www.rm.dk/siteassets/om-os/aktuelt/2019/05-maj/udgifter-til-indflytning-og-ibrugtagning-af-dnu-070519.pdf>

### Storstrømsbroen (Dronning Margrethe II's Bro)

-   <https://www.ft.dk/samling/20201/almdel/TRU/bilag/372/2401915/index.htm>

### Ejendomsvurderingssystemet (ICE)

-   <https://cdn.rigsrevisionen.dk/rigsrevisionen/Media/638998268925610237/1509-25.pdf>
-   <https://rigsrevisionen.dk/Media/638998268925610237/1509-25.pdf>

### Niels Bohr Bygningen

-   <https://bygst.dk/media/plfgvcwt/erfaringsrapport-niels-bohr-bygningen.pdf#page=5.15>

### Lynetteholm (halvø/perimeter)

-   <https://byoghavn.dk/wp-content/uploads/2019/04/Bilag-vedr.-samlet-anlaegsbudget-og-businesscase-for-etab-lering-af-Lynetteholm_2022.pdf>

### Energiø Bornholm

-   <https://www.dr.dk/nyheder/indland/byggeriet-af-landanlaeg-til-energioe-bornholm-spraenger-budgettet>
-   <https://www.dr.dk/nyheder/politik/pausen-er-aflyst-regeringen-giver-groent-lys-til-stor-kontrakt-om-energioe-bornholm>

### Odense Letbane (etape 1)

-   <https://danskejernbaner.dk/vis.bane.php?BANE_ID=215>
-   <https://odenseletbane.dk/alt-om-letbanen/tal-og-fakta>
-   <https://www.tv2fyn.dk/odense/her-er-de-vilde-tal-bag-odense-letbane>

### Aarhus Letbane (etape 1)

-   <https://danskejernbaner.dk/vis.bane.php?BANE_ID=248>

### Femern Bælt-forbindelsen (kyst-til-kyst)

-   <https://www.ft.dk/samling/20211/almdel/tru/bilag/140/2514319.pdf>
-   <https://www.dr.dk/nyheder/seneste/femern-tunnelen-bliver-mindst-aar-forsinket>

### Aarhus Stadion (Kongelunden)

-   <https://www.tv2ostjylland.dk/aarhus/nyt-stort-millionbelob-til-skandaleramt-stadionbyggeri-fe138>
-   <https://dansk-byudvikling.dk/nyt-stadion-i-aarhus-endnu-en-forsinkelse-truer/>
-   <https://www.dr.dk/nyheder/indland/millionbesparelser-paa-aarhus-nye-stadion-enighed-om-faerre-siddepladser-men-vip>

### Tunnel under Marselis Boulevard, Aarhus

-   <https://dinavis.dk/samfund/ECE17621891/prisen-paa-aarhustunnel-er-eksploderet-og-det-kan-blive-vaerre>
-   <https://altinget.dk/artikel/endnu-et-vejprojekt-i-statens-byggeplan-giver-milliardunderskud-efter-fordyrelser>

### Mary Elizabeths Hospital (BørneRiget)

-   <https://www.dr.dk/nyheder/indland/budgetoverskridelse-boernehospital-paa-riget-skal-bruge-661-millioner-ekstra>
-   <https://via.ritzau.dk/pressemeddelelse/14533455/budgettet-pa-mary-elizabeths-hospital-oges-med-795-mio-kr>
-   <https://sundhedspolitisktidsskrift.dk/nyheder/sundhedspolitik/10501-budget-for-nyt-bornehospital-skrider-igen-denne-gang-med-naesten-en-milliard-kroner.html>

### Hovedstadens Letbane

-   <https://dinletbane.dk/da/nyheder/anlaegsbudget-for-hovedstadens-letbane-er-nu-kortlagt/>
-   <https://www.tv2kosmopol.dk/koebenhavn/ramt-af-saerlige-udfordringer-letbanestraekning-i-hovedstaden-forsinkes>
-   <https://www.dr.dk/nyheder/indland/nyaabnet-letbane-forventer-langt-faerre-passagerer-end-da-det-blev-besluttet-bygge-den>

### Signalprogrammet (ERTMS)

-   <https://ing.dk/artikel/milliarder-over-budget-og-12-aar-forsinket-ny-kaempe-check-skal-redde-kriseramte-togsignaler>
-   <https://bane.dk/da/Presse/Pressemeddelelser/Ny-udrulningsplan-paa-plads-for-det-digitale-signalsystem-i-OEstdanmark>
-   <https://nyheder.tv2.dk/trafik/2026-07-22-nye-tal-afsloerer-hundredvis-af-signalfejl-ekspert-er-rystet>

### Prisindeks fra Økonomistyrelsen

-   [Økonomistyrelsen -- Regulering af
    anlægsprojekter](https://oes.dk/statsregnskab/finanslov-og-udgiftsopfoelgning/indeks/regulering-af-anlaegsprojekter/)
