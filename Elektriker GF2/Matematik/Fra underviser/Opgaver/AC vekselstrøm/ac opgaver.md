
### Opgave 2
![[Pasted image 20261006083205.png]]

#### a) Tegn vektordiagram

![[Pasted image 20261006084103.png|330]]
#### b) Beregn kapacitansen
XC= ??? = kapacitansen, den kapacitive modstand [Ω]
C = $31,83\mu F$ = Kondensatorens kapacitet (kapacitansen) [μF]
$R = 120ohm$
U = 230V
f = 50 Hz

$XC = \frac{10^6}{2*\pi*f*C} \implies XC =\frac{10^6}{2*\pi*50*31.83}= 100.003\ldots$
Formlen tager højde for at C bliver målt i $\mu F$

#### c) Beregn kredsens impedans
Z = impedans (samlet modstand) [Ω]

XC = 100ohm i -90deg vinkel
XR = 120ohm i 0deg vinkel

$Z = XC+XR = (100\angle -90\degree)+(120\angle 0\degree)= 20\sqrt{61}\angle 320.194\degree \approx 156.205\angle 320.194\degree$
den samlede impedans er lig = 156.2 ohm
Faseforskydningen er = $320.2\degree$ også kaldet $\phi$ 

#### d) Cos $\phi$
$\cos(320.2\degree)= 0.768283523593523376273$

#### e) Det ohmske spændingsfald + f) Det kapacitive spændingsfald

##### Forregning
R = 156.2 ohm
U = 230V

$I=\frac{U}{R}=\frac{230}{156.2}= 1.473A$

##### Ohmske spændingsfald
Eftersom forbindelsen er i serie har jeg her regnet strømmen eftersom den er konstant 
Så nu kan jeg regne det samlede spændingsfald

$UR=R*I=120*1.473= 176.76V$
Dette er spændingsfaldet over den ohmske modstand på 120ohm

##### Det kapacitive spændingsfald
Nu skal jeg finde modstanden over kondenstatoren som jeg ved XC = 100ohm fra b)
$UC=R*I=100*1.473= 147.3V$

##### Det samlede spændingsfald
Nu skal de lægges sammen med højde for deres vinkel
XC = 100ohm i -90deg vinkel
XR = 120ohm i 0deg vinkel
$U_{R}+U_{C}=176.76\angle_{0\degree}+147.3\angle-90\degree= 230.09\ldots\angle 320.194\degree$

den samlede spændingsfald er lig = 230.09V 
Faseforskydningen er = $320.194\degree$ 

### Opgave 3
![[Pasted image 20261006094128.png]]

XR = 80ohm -> $0\degree$
L = 0.2 H
C = $50\mu F$
$U_{tot}=230V$
f = 50Hz
#### a) Tegn vektordiagram
![[Pasted image 20261006101821.png|341]]
#### b) Impedansen
Inden jeg kan regne impedancen skal jeg finde modstanden over xL og C
$XL=2*\pi*f*L=2*\pi*50*0.2\approx 62.831ohm\angle {90}\degree$
$XC=\frac{10^6}{2*\pi*f*C}=\frac{10^6}{2*\pi*50*50}\approx 63.661ohm\angle-90\degree$

Med disse 2 modstande samt den opgivne modstand kan vi nu finde impedansen:
$Z = XR+XL+XC=80\angle0\degree+62.831\angle90\degree+63.661\angle-90\degree = 80.004\ldots\angle 359.406\degree$

#### c) Strømmen i kredsen
Strømmen i kredsen kan nu regnes med den opgivne spænding og Z
$I=\frac{U}{Z}=\frac{230}{80}\approx 2.875A$

#### d) Spændingerne $UR_{s}-UL-UC$
Nu skal vi dele spændingsfaldet op over diverse modstand UR UL UC
Strømmen er konstant i en serieforbindelse: 
I = 2.875A
$XR=80ohm\angle_{0}\degree$
$XL=62.831ohm\angle{90}\degree$
$XC=63.661ohm\angle{-90}\degree$

$UR=80*2.875= 230$
$UL=62.831*2.875= 180.639125$
$UC=63.661*2.875= 183.025375$

$U=UR+UL+UC=230\angle{0}\degree+180.64\angle{90}\degree+183.03\angle-90\degree\approx 230.012\ldots\angle 359.405\degree$
#### e) Effekterne S-P-Q
![[Pasted image 20261006110345.png]]
Hvergang man skal til venstre i disse 3-kanter skal man gange med I her er vinkler ikke vigtige eftersom de stadig fortsætter med deres retning
$Z*I=U\implies U*I=S$
$80*2.875= 230*2.875= 661.25VA$

$R*I=UR \implies UR*I=P$
$80*2.875= 230*2.875= 661.25W$

$XL*I=UL\implies UL*I=Q$
Inden jeg kan bruge XL skal XL og XC ligges sammen
$XL+XC=62.831\angle{90}\degree+63.661\angle{-90}\degree= 0.83\angle 270\degree$
$0.83*2.875= 2.38625*2.875= 6.86046875VAr$
#### f) cos $\phi$ 
$\cos(359.406\degree)= 0.999946260485365538364$


### Opgave 5
![[Pasted image 20261006112356.png]]
XR = 120ohm -> $0\degree$
C = $25\mu F$
$U_{tot}=230V$
f = 50Hz

#### a) Tegn vektordiagram
Kondensator er 90deg når den er i paralel men -90deg i serie
![[Pasted image 20261006113933.png]]
#### b) Impedansen
Impedans skrives som XC
$XC =\frac{10^6}{2*\pi*f*C}=\frac{10^6}{2*\pi*50*25}\approx 127.323\ldots$
Kondensatorens modstand er derfor 127.323ohm
Den samlede modstand i paralel regnes som følgende:
$XC=\frac{1}{\left( \frac{1}{(127.323\angle{90}\degree)} \right)+\left( \frac{1}{(120\angle{0\degree})} \right)}=87.33ohm\angle{43.3}\degree$



#### c) Den samlede strøm

$I=\frac{U}{R}=\frac{230}{87.33}= 2.63A$


#### d) Strømmen igennem kondensatoren - Ic
Spændingen er konstant på 230
Modstanden i kondensatoren er 127.323ohm
$\frac{230}{127.323}= 1.80642931756241998696$
#### e) Strømmen igennem modstanden - Iv
Spændingen er konstant på 230
Modstanden er 120 ohm
$\frac{230}{120}\approx 1.916\ldots$

#### f) cos $\phi$
$\cos(43.3)= 0.776126236378924370142$


### Opgave 6
![[Pasted image 20261006122319.png]]
![[Pasted image 20261006122536.png]]

#### a) tegn vektordiagram
#### b) den samlede strøm

#### c) faseforskydningsvinklen
#### d) effekterne S-P-Q

### Opgave 7
![[Pasted image 20261006122610.png]]
![[Pasted image 20261006122624.png]]

### Opgave 8
![[Pasted image 20261006122714.png]]
![[Pasted image 20261006123719.png|347]]

Fordi det er en serie er strømmen konstant så jeg kan nøjes med at bruge 1 modstand sammen med spændingen
b):
$I=\frac{U}{R}=\frac{200}{55}\approx 3.636\ldots$

c):
$XL=2*\pi*f*L=2*\pi*50*0.27\approx 84.823ohm$




### Opgave 9
![[Pasted image 20261006122917.png]]

Rs = 25ohm
R = 15ohm
$U_{tot}=230V$
f = 50Hz
L = 0.15H
$XL=2*pi*f*L=2*\pi*50*0.15\approx 47.123\ldots$ohm

#### a)
![[Pasted image 20261021085130.png|260]]
$Z_{s}=(25\angle0\degree)+(47.123\angle 90\degree)\approx 53.344ohm\ldots\angle 62.053\degree$


![[Pasted image 20261021090456.png|293]]



 
#### b)
![[Pasted image 20261021091134.png|416]]


#### c)
Nu ligges strømmen fra spolen og strømmen fra modstanden sammen.

$I_{s}=\frac{230}{47.123}\approx 4.880A\ldots$
$I_{R}=\frac{230}{15}\approx 15.333A$

$I_{tot}=I_{S}+I_{R}=4.880+15.333= 20.213A$

#### d)
$(4.88\angle-62\degree)+(15.33\angle 0\degree)= 18.14\ldots\angle 346.259\degree$
$\cos(346.259\degree)= 0.971$

#### e)
$Z_{s}=(25\angle0\degree)+(47.123\angle 90\degree)\approx 53.344ohm\ldots\angle 62.053\degree$



### Opgave 10
![[Pasted image 20261006122932.png]]
