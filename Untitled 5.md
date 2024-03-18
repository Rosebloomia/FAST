Vypočtěte nejnižší povrchovou teplotu $\Theta_{si,min}$ a teplotní faktor vnitřního povrchu $f_{Rsi}$
- v konstrukcích S1s, S1n, P1s, P1n
- ve svislých koutech S1s - S1s, S1n - S1n
- ve vodorovných koutech P1s - S1s, P1n - S1n
Posuďte normovými hodnotami.
Okrajové podmínky:
- $\Theta_i = 20°C$
- $\Theta_{ai} = \Theta_i + \Delta \Theta_{ai}=20+0.6=20.6°C$
- $\varphi_i = 50\%$
- $\Theta_e = -13°C$
- $R_{si} = 0.25\ m^2.K.W^{-1}$ pro výpočty šíření vlhkosti (tabulka J.1, sloupec 4)
- $\Theta_{sut} = 10°C$ 
## Postup výpočtu
##### 1.\ V ploše:

Nejnižší povrchová teplota $\Theta_{si,min}$
$$\large \Theta_x=\Theta_{ai}-U\cdot R_{x}\left(\Theta_{ai}-\Theta_{e} \right)\ \ \ \ [°C]$$
$$\large \Theta_{si,min}=\Theta_{ai}-U\cdot R_{si}\left(\Theta_{ai}-\Theta_{e} \right)\ \ \ \ [°C]$$
Teplotní faktor vnitřního povrchu $f_{Rsi}$
$$f_{Rsi} = \frac{\Theta_{si,min}-\Theta_e}{\Theta_{ai}-\Theta_e}\ \ \ [-]$$
##### 2.\ V koutě:

Nejnižší povrchová teplota $\Theta_{si,min}
$$\Theta_{si,min} = \Theta_{ai} - \xi_{Rsi}\cdot \left( \Theta_{ai}-\Theta_e \right)\ \ \ [°C]$$
- $\xi_{Rsi}$ - poměrný teplotní rozdíl vnitřního povrchu v koutě $[-]$
    - kout mezi vnějšími konstrukcemi: $\xi_{Rsi}=1.05\cdot\left(U\cdot R_{siK} \right)^{0.69}\ \ \ [-]$
    - kout mezi vnitřními konstrukcemi: $\xi_{Rsi}=0.6\cdot\left(U\cdot R_{siK} \right)^{0.79}\cdot\left(\frac{U_e}{U_i}\right)^{0.21}\ \ \ [-]$
$R_{siK}$ - tepelný odpor při přestupu tepla v koutě $[m^2.K.W^{-1}]$ podle tab J.1 ČSN 73 0540-3:2005
Postup je přípustný, pokud platí $0.8\le \frac{U_1}{U_2}\le 1.25$
Teplotní faktor vnitřního povrchu $f_{Rsi,min}$
$$f_{Rsi} = 1 - \xi_{Rsi}\ \ \ [-]$$
Musí platit:
- $f_{Rsi}\ge f_{Rsi,N}$, kde $f_{Rsi,N}$ je normový teplotní faktor vnitřního povrchu
- $f_{Rsi,N}=f_{Rsi,cr}$ kde $f_{Rsi,cr}$ je kritický teplotní faktor vnitřního povrchu \[-] podle tab. 1 ČSN 73 0540-2:2011 + Z1:2012 pro standardní okrajové podmínky, jinak výpočtem