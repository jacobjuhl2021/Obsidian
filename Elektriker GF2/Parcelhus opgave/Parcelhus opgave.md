
#### RCD
2x Type A
1x Type B til ladeboks og varmepumpe

**Hvorfor Type B?**
- RCD’er (Residual Current Devices eller fejlstrømsafbrydere) af type A kan kun detektere a.c. og pulserende d.c. samt d.c.-reststrømme op til 6 mA.
- Hvis RCD’en skal kunne detektere d.c.-reststrømme over 6 mA, skal man anvende en type B-afbryder. 

**Hvorfor Type A?**
- Er alment brugt i boliger. 60364 angiver der skal beskyttes mod reststrømme, samt DC-reststrømme

**Hvorfor flere?**
- Krav i 60364 at en enkel fejl i installationen ikke skal kunne slukke strømmen i hele boligen

[Sikkerhedsstyrelsen valg af RCD](https://www.sik.dk/erhverv/elinstallationer-og-elanlaeg/vejledninger/elinstallationer/eltavler-og-maalertavler/valg-og-installation-rcd-fejlstroemsafbryder)
[Sikkerhedsstyrelsen spørgsmål og svar om RCD](https://www.sik.dk/erhverv/elinstallationer-og-elanlaeg/sporgsmal-og-svar/elinstallationer/sporgsmal-og-svar-om-beskyttelse-med-rcder)

#### Fordeling af grupper
3 lysgrupper [[BEK 1082.pdf#page=7&selection=73,0,73,4|BEK 1082 §56 Antal Grupper]] [[BEK 1082.pdf#page=7&selection=105,0,105,4|BEK 1082 §57 Antal 230V stikkontakter]]
4 kraftgrupper (Ladeboks, Varmepumpe, Køkken og kraftgruppe til garage)

**Lysgruppe 1 10A Bryggers, Værelse 1, Værelse 2, Entre/Gang, bad, depot**
	et værelse bruger 650 watt $\frac{650W}{230V}= 2.826A$ ved maks forbrug
	da vi har to værelser så $2.826A*2= 5.652A$
	forbrug i bad, bryggers, entre og depot er minimalt ift de to værelser så de kan sagtens forsynes fra samme gruppe.

**Lysgruppe 2 10A Køkken, K/A, Soveværelse, Bad 2**
	køleskab maks. strømforbrug: $\frac{200W}{230V}= 0.869A$
	fryser maks. strømforbrug: $\frac{250W}{230V}= 1.086A$
	stikkontakter
	lys

**Lysgruppe 3 16A Køkken**
	ovn maks. strømforbrug: $\frac{3000W}{230V}= 13.043A$
	stikkontakter

**Kraftgruppe 1 16A Induktionskogeplade/Køkken**

**Kraftgruppe 2 16A Ladeboks**

**Kraftgruppe 3 16A Varmepumpe**


**Kraftgruppe 4 16A Garage**
	L1: Kraftstik, Stikontakter, Udendørsbelysning, Lys Garage
	L2: Kraftstik, Tørretumbler
	L3: Kraftstik, Vaskemaskine
	bryggers hvis vaskemaskine og tørretumbler kører samtidigt
		$P_{tørretumbler}=2500W$
		$P_{Vaskemaskine}=2000W$
		$P=\frac{2500W+2000W}{230V}= 19.565A$

#### Stikkontakter
Valg af antallet af stikkontakter [[BEK 1082.pdf#page=7&selection=105,0,105,4|BEK 1082 §57 Antal 230V stikkontakter]]
**Værelse 1:** $\frac{10.35m^2}{4m^2}= 2.587$ så 3 stikkontakter
**Værelse 2:** $\frac{10m^2}{4m^2}= 2.5$ så 3 stikkontakter
**Soveværelse:** $\frac{9.9m^2+3.45m^2}{4}= 3.337$ så 4 stikkontakter
**K/A:** $\frac{46.45}{4}= 11.612$ så minimum 10 stikkontakter(min. 3 i køkken)
**Bryggers:** $\frac{8.35m^2}{4m^2}= 2.087$ så 3 stikkontakter
**Bad 1 & 2:** minimum 1, vi vælger 3 stikkontakter
**Garage:** Ikke noget krav, vi vælger 4
**Udendørs:** Ikke noget krav, vi vælger 2 stikkontakter


#### [[Dimensionering#Dimensionering af Stikledning|Stikledning]]
[Sikkerhedsstyrelsen simpel dimensionering](https://www.sik.dk/erhverv/elinstallationer-og-elanlaeg/vejledninger/elinstallationer/dimensionering-elektriske-installationer/simpel-dimensionering-installationer#:~:text=HD%2060364%2Dserien.-,Tabel%20til%20simpel%20dimensionering,-Ledertv%C3%A6rsnit%20(mm%C2%B2)%20kobber)
Vi bruger simpel dimensionering, vi har 25A i gravstenen så stikledningen skal have et tværsnit på $10mm^2$ $CU$

#### [[Dimensionering#Dimensionering af Jord|Jording]]
##### Hovedjordingsforbindelse/Beskyttelseslederen
jf. [[60364 version 11_2026.pdf#page=424&selection=19,0,21,21|543.1 Mindste Ledertværsnit]] skal beskyttelseslederen være samme størrelse som stikledningen
##### Beskyttende potentialudligning
jf. [[60364 version 11_2026.pdf#page=429&selection=61,4,63,69|544.1]] skal vi bruge $6mm^2$ $CU$
Skal forbindes til rionet og VVS rør
##### Supplerende beskyttende potentialudligning
jf. [[60364 version 11_2026.pdf#page=425&selection=55,0,55,7|543.1.3]] skal vi bruge $2.5mm^2$ $CU$
Skal installeres til stikkontakter og VVS rør i badeværelserne





