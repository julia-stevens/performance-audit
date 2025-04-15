# Performance Audit 

Doe een Performance audit op een bestaande website uit je eigen omgeving en rapporteer daarover.

De instructies van deze opdracht staan in [INSTRUCTIONS](https://github.com/fdnd-task/performance-audit/blob/main/docs/INSTRUCTIONS.md).
 

## Het Streek Lyceum
### Inleiding
Schrijf een samenvatting van de testbevindingen, en link naar je Wiki voor de volledige documentatie van je onderzoek.

Voor deze deeltaak test ik de website van mijn middelbare school, namelijk: [Het Streek Lyceum](https://www.hetstreek.nl/lyceum/)

<img width="800" alt="image" src="https://github.com/user-attachments/assets/4aad3873-bdfa-4948-994c-9720989763fe" />

[Zie de Wiki voor de volledige documentatie](https://github.com/julia-stevens/performance-audit/wiki/Deeltaak:-Performance-Audit)

### Lighthouse test
#### Mobile
##### Resultaat
<img width="800" alt="image" src="https://github.com/user-attachments/assets/c73321c2-34ce-4302-9cf7-b2feaf0a1a3d" />

#### Desktop
##### Resultaat
<img width="800" alt="image" src="https://github.com/user-attachments/assets/ee6127cc-9550-46a1-b41f-901d6ff4af61" />

#### Verschillen tussen mobile en desktop
- Verschillen tussen mobile en desktop Lighthouse test
- Langzame LCP - grootste element wordt laat ingeladen op mobiel
- Veel render-blocking resources - op mobiel gebeurt dit meer dan op desktop
- Langzame initial server response - server reageert trager op mobiel
- JS scripts draaien langzamer op mobiel
- Veel grote afbeeldingen die langer laden op mobiel
- Externe scripts zorgen voor vertraging op mobiel

### PageSpeed Insights
#### Resultaten 
##### [Mobile](https://pagespeed.web.dev/analysis/https-www-hetstreek-nl-lyceum/us9aupahum?form_factor=mobile)
<img width="800" alt="image" src="https://github.com/user-attachments/assets/b5835dd6-1747-427a-abae-d96c8b5174f3" />

##### [Desktop](https://pagespeed.web.dev/analysis/https-www-hetstreek-nl-lyceum/us9aupahum?form_factor=desktop)
<img width="800" alt="image" src="https://github.com/user-attachments/assets/b99ec453-a470-4d1e-9357-b26b652ff044" />

#### Verschillen tussen Lighthouse test en PageSpeed Insights
Het verschil in performance is aanzienlijk, dit zijn mogelijke oorzaken:
- PageSpeed Insights werkt met zwaardere throttling
- Lighthouse draait vaak lokaal en resultaten zijn dus beter dan de resultaten van echte gebruikers (PageSpeed Insights)

#### CrUX 
##### Mobile en desktop
<img width="600" alt="image" src="https://github.com/user-attachments/assets/10d42338-1a0d-4a4e-9213-e41395a2a180" />

### Webpage test
#### Bevindingen 
De website laadt traag door blokkerende JavaScript-bestanden, grote en trage SVG's, en externe bronnen zoals YouTube en Google Fonts. Daarnaast veroorzaken meerdere 404's vertraging, en is het totale aantal HTTP-verzoeken hoog, wat de performance negatief beïnvloedt.

#### Waterfall chart
[Bekijk resultaten](https://www.webpagetest.org/result/250415_AiDc6S_B75/1/details/#waterfall_view_step1)

![waterfall](https://github.com/user-attachments/assets/68b36e79-9932-4f87-92cc-8941e531e8e7)

## Licentie

This project is licensed under the terms of the [MIT license](./LICENSE).
