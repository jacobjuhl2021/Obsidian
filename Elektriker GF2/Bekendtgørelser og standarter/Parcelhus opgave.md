#### Kunde
Familie 2 børn, som gamer
Varmepumpe, ladeboks til elbil.
Manden rode i garagen, så der skal bruges kraftstik.

Allerede kan man se at denne familie generelt kommer til at bruge mere strøm end den gennemsnitlige.

#### RCD
2x Type A
1x Type B til ladeboks og varmepumpe

**Hvorfor Type A?**
- Er alment brugt i boliger. 60364 angiver der skal beskyttes mod reststrømme, samt DC-reststrømme
**Hvorfor Type B?**
- RCD’er (Residual Current Devices eller fejlstrømsafbrydere) af type A kan kun detektere a.c. og pulserende d.c. samt d.c.-reststrømme op til 6 mA.
- Hvis RCD’en skal kunne detektere d.c.-reststrømme over 6 mA, skal man anvende en type B-afbryder. 
**Hvorfor flere?**
- Krav i 60364 at en enkel fejl i installationen ikke skal kunne slukke strømmen i hele boligen

[Sikkerhedsstyrelsen valg af RCD](https://www.sik.dk/erhverv/elinstallationer-og-elanlaeg/vejledninger/elinstallationer/eltavler-og-maalertavler/valg-og-installation-rcd-fejlstroemsafbryder)
[Sikkerhedsstyrelsen spørgsmål og svar om RCD](https://www.sik.dk/erhverv/elinstallationer-og-elanlaeg/sporgsmal-og-svar/elinstallationer/sporgsmal-og-svar-om-beskyttelse-med-rcder)

#### Fordeling af grupper
3 lysgrupper 
[[BEK 1082.pdf#page=7&selection=73,0,73,4|BEK 1082 §56 Antal Grupper]] 
[[BEK 1082.pdf#page=7&selection=105,0,105,4|BEK 1082 §57 Antal 230V stikkontakter]]
[[BEK 1082.pdf#page=7&selection=115,0,120,30|BEK 1082 $56 stk. 2]] (Køkken fordeles på 2 grupper)
4 kraftgrupper (Ladeboks, Varmepumpe, Køkken og kraftgruppe til garage)

**Lysgruppe 1 10A Bryggers, Værelse 1, Værelse 2, Entre/Gang, Bad 1, Depot**
	et værelse bruger 650 watt $\frac{650W}{230V}= 2.826A$ ved maks forbrug
	da vi har to værelser så $2.826A*2= 5.652A$
	forbrug i bad, bryggers, entre og depot er minimalt ift de to værelser så de kan sagtens forsynes fra samme gruppe.

**Lysgruppe 2 10A Køkken, Soveværelse, Bad 2**
	køleskab maks. strømforbrug: $\frac{200W}{230V}= 0.869A$
	fryser maks. strømforbrug: $\frac{250W}{230V}= 1.086A$
	stikkontakter
	lys (Soveværelse, Bad 2)

**Lysgruppe 3 10A Køkken, K/A**
	lys
	stikkontakter
	emhætte

**Kraftgruppe 1 16A Induktionskogeplade/Ovn/Køkken**
	L1: Induktionskogeplade
	L2: Induktionskogeplade
	L3: Ovn

**Kraftgruppe 2 16A Ladeboks**

**Kraftgruppe 3 16A Varmepumpe**

**Kraftgruppe 4 16A Garage/Vaskemaskine/Tørretumbler/Udendørs**
	L3: Kraftstik, Vaskemaskine
	L2: Kraftstik, Tørretumbler
	L1: Kraftstik, Stikontakter, Udendørsbelysning, Lys Garage
	bryggers hvis vaskemaskine og tørretumbler kører samtidigt
		$P_{tørretumbler}=2500W$
		$P_{Vaskemaskine}=2000W$
		$P=\frac{2500W+2000W}{230V}= 19.565A$

#### Tavle opbygning
**#1 RCD Type A**
	Kraftgruppe 4 16A
	Lysgruppe 1 10A

**#2 RCD Type A**
	Kraftgruppe 1 16A
	Lysgruppe 2 10A
	Lysgruppe 3 10A

**#3 RCD Type B**
	Kraftgruppe 2 16A
	Kraftgruppe 3 16A

#### Stikkontakter
Valg af antallet af stikkontakter [[BEK 1082.pdf#page=7&selection=105,0,105,4|BEK 1082 §57 Antal 230V stikkontakter]]
**Værelse 1:** $\frac{10.35m^2}{4m^2}= 2.6$ så 3 stikkontakter
**Værelse 2:** $\frac{10m^2}{4m^2}= 2.5$ så 3 stikkontakter
**Soveværelse:** $\frac{9.9m^2+3.45m^2}{4m^2}= 3.337$ så 4 stikkontakter
**K/A:** $\frac{46.45m^2}{4m^2}= 11.612$ så minimum 10 stikkontakter(min. 3 i køkken)
	**Køkken:** 12 stikkontakter (7 disp.)
	**Opholdsstue:** 7 stikkontakter
**Bryggers:** $\frac{8.35m^2}{4m^2}= 2.087$ så 3 stikkontakter
**Bad 1 & 2:** minimum 1, vi vælger 3 stikkontakter
**Garage:** Ikke noget krav, vi vælger 5 stikkontakter + 1 kraftstik
**Udendørs:** Ikke noget krav, vi vælger 2 stikkontakter
**Entre/Gang:** $\frac{9.45}{4}= 2.362$, mindst 3 stikkontakter vi vælger 4
**Depot:** Ikke krav til stikkontakt, men vi vælger 1


#### [[Dimensionering#Dimensionering af Stikledning|Stikledning]]
[Sikkerhedsstyrelsen simpel dimensionering](https://www.sik.dk/erhverv/elinstallationer-og-elanlaeg/vejledninger/elinstallationer/dimensionering-elektriske-installationer/simpel-dimensionering-installationer#:~:text=HD%2060364%2Dserien.-,Tabel%20til%20simpel%20dimensionering,-Ledertv%C3%A6rsnit%20(mm%C2%B2)%20kobber)
Vi bruger simpel dimensionering.
Da vi har en ret høj mærkestrøm, skal vi bruge 50A sikringer ude i gravstenen.
50A er ikke på diagrammet, men da vi er gået 2 størrelser op fra 25A går vi også 2 størrelser op i stikledning.

Så vi har fremskrevet diagrammet for simpel dimensionering, og lander på et tværsnit for **stikledningen** på $25mm^2$

#### [[Dimensionering#Dimensionering af Jord|Jording]]
##### Hovedjordingsforbindelse/Beskyttelseslederen
jf. [[60364 version 11_2026.pdf#page=424&selection=19,0,21,21|543.1 Mindste Ledertværsnit]] skal beskyttelseslederen have en størrelse på $16mm^2$
##### Beskyttende potentialudligning
jf. [[60364 version 11_2026.pdf#page=429&selection=61,4,63,69|544.1]] skal vi br uge $8mm^2$ $CU$, da den beskyttende potential udligning skal være halv størrelse af den største [[Parcelhus opgave#Hovedjordingsforbindelse/Beskyttelseslederen|beskyttelsesleder]]
Skal forbindes til rionet og VVS rør
##### Supplerende beskyttende potentialudligning
jf. [[60364 version 11_2026.pdf#page=425&selection=55,0,55,7|543.1.3]] skal vi bruge $2.5mm^2$ $CU$ (Installeres så der ikke er risiko for mekanisk beskadigelse)
Skal installeres til stikkontakter og VVS rør i badeværelserne



#### Beregning af spændingsfald
Spændingsfald udregnes sådan: $\Delta U=R_{L}*I_{B}$
Ledningsmodstanden udregnes sådan: $R_{L}=\frac{\rho*l*2}{q}$
Strømmen for brugsgenstanden udregnes sådan: $I_{B}=P_{B}*U_{B}$

Vi kan substituere $R_{L}$ og $I_{B}$ i formlen for spændingsfald og får
$\Delta U=R_{L}*I_{B}\implies\frac{\rho*l*2}{q}* \frac{P_{B}}{U_{B}}\implies$
$$\Delta U=\frac{\rho*2}{q*U_{B}}*l*P_{B}$$
$\frac{\rho*2}{q*U_{B}}$ er en konstant og kan udregnes for både lysgrupperne og kraftgrupperne og kaldes for $k$. Ved lysgrupper bruger vi $1.5mm^2$, og ved kraftgrupper bruger vi $4mm^2$
$k_{kraft}=\frac{0.0225*2}{4*400}=\frac{0.045}{1600}$
$k_{lys}=\frac{0.0225*2}{1.5*230}=\frac{0.045}{345}$
formlen hedder nu:
$$
\Delta U=k*l*P_{B}
$$

##### Lysgruppe 1 (Værelse 1)
$\Delta U_{\text{Værelse 1}}=k_{lys}*l*P_{B}=\frac{0.045}{345}*10m*650W\approx 0.847V$
$\Delta U\%_{\text{Værelse 1}}=\frac{0.847V}{230V}= 0.00368=0.368\%$

##### Lysgruppe 2 (Elkedel)
$\Delta U_{\text{Elkedel}}=k_{lys}*l*P_{B}=\frac{0.045}{345}*21m*2200W\approx 6.026V$
$\Delta U\%_{elkedel}=\frac{6.026V}{230V}= 0.0262=2.62\%$

##### Lysgruppe 3 (paninigrill)
$\Delta U_{\text{Paninigrill}}=k_{lys}*l*P_{B}=\frac{0.045}{345}*21m*1600W\approx 4.382V$
$\Delta U\%_{\text{Paninigrill}}=\frac{4.382V}{230V}\approx 0.019=1.9\%$

##### Kraftgruppe 1 16A (Induktionskogeplade)
$\Delta U_{\text{Kogeplade}}=\frac{0.045}{1600}*25m*11*10^3W= 7.734V$
$\Delta U\%=\frac{7.734V}{400V}= 0.019=1.9\%$

##### Kraftgruppe 2 16A (Ladeboks)
Afstand fra tavle til ladeboks: $5.5m$
Effekten for ladeboksen er på $11kW$
Vi bruger $4mm^2$ $CU$
Spændingsfaldet udregnes sådan: $\Delta U=R_{L}*I_{B}$
Ledningsmodstanden udregnes sådan: $R_{L}=\frac{\rho*l*2}{q}=\frac{0.0225 \frac{\Omega*mm^2}{m}*5.5m*2}{4mm^2}= 0.061\Omega$
Strømmen for ladeboksen udregnes sådan: $I_{B}=\frac{P_{B}}{U_{B}}=\frac{11*10^3W}{400V}= 27.5A$
Nu kan spændingsfaldet udregnes: $\Delta U=R_{L}*I_{B}=0.061\Omega*27.5A= 1.677V$
Spændingsfald i % udregnes sådan: $\Delta U\%=\frac{\Delta U}{U_{net}}=\frac{1.677V}{400V}= 0.004=0.4\%$
Er langt under de tilladte 5%


##### Kraftgruppe 3 16A (Varmepumpe)
Varmepumpen har en effekt på $8kW$
Varmepumpens ledning har en længde på 15m
$\Delta U_{\text{Varmepumpe}}=k_{kraft}*l*P_{B}=\frac{0.045}{1600}*15m*8*10^3W= 3.375V$
$\Delta U_{\text{Varmepumpe}}\%=\frac{3.375V}{400V}\approx 0.008=0.8\%$
Varmepumpen har et spændingsfald på $0.8\%$

##### Kraftgruppe 4 16A (Svejser i kraftstik)
$\Delta U_{\text{Svejser}}=k_{kraft}*l*P_{B}=\frac{0.045}{1600}*15m*11*10^3W\approx 4.640V$
$\Delta U\%_{\text{Svejser}}=\frac{4.640V}{400V}= 0.0116=1.16\%$

##### [[60364 version 11_2026.pdf#page=324&selection=13,0,13,28|60364 Tabel G.52.1 Tilladt mængde spændingsfald]]
![[Pasted image 20260930105456.png]]

#### Udendørs installation
[[BEK 1082.pdf#page=6&selection=8,0,8,4|BEK 1082 §41 Nedgravning af kabler]]
[[60364 version 11_2026.pdf#page=706&selection=16,0,20,37|60364 Installation af udendørs elektrisk materiel]]
