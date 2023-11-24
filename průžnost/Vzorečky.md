```ad-attention
title: Jednotky

## KN/m/KPa        - střední / střední / střední
---
## N/mm/MPa        - malý / malý / bigass
```
## Napětí $\large\sigma x$
$$\large\sigma x=\frac{N}{A}\ \ \ [KPa]$$
- $N$ - síla ($Kn$)
- A - plocha ($m$)

## Deformace (prodloužení) $\large\Delta l$
$$\large\Delta l=\frac{N\cdot l}{E\cdot A}\ \ \ \ [m]$$
- $N$ - síla ($KN$)
- $l$ - délka ($m$)
- $E$ - modul pružnosti ($KPa$)

## Teplotní deformace $\large\Delta l$
$$\large\Delta l=\alpha\cdot l_{0}\cdot \Delta t\ \ \ \ [m]$$
- $\alpha$ - koeficient teplotní roztažnosti (např. $1.2 \cdot 10^{-6}K^{-1}$)
- $l_0$ - původní délka materiálu (m)
- $\Delta t$ - teplotní změna (v kelvinech, takže to samé jak celsius jen jiná nula)

## Napětí za ohybu
$$\large \sigma x = \frac{M_y}{I_{y}}\cdot z\ \ \ \ [KPa]$$
- $M_y$ - moment v místě průřezu ($Kn\cdot m = Kpa$)
- $Iy$ - moment setrvačnosti ($m^4$) - při výpočtu dosazovat metry
- $z$ - vzdálenost od těžiště ($m$), většinou k okraji průřezu, **nahoru je *-* dolů je +**

## Smykové napětí za ohybu
$$\large \tau_{xz} = \frac{V_z\cdot S_y}{I\cdot b}\ \ \ \ [KPa]$$
- $V_z$ - posouvající síla ($KN$) v požadovaném místě, většinou největší od 0
- $S_y$ - statický moment ($m^4$) odřezané části, dosazujeme v metrech
- $I$ - moment setrvačnosti ($m^4$)
- $b$ - šířka v místě řezu ($m$)

## Statický moment
$$\large S_y =  A\cdot z_y$$
- $A$ - plocha ($m^2$)
- $z_y$ - vzdálenost od těžištní osy ($m$)

## Šikmý ohyb
$$\large \sigma x= \frac{M_{y}^*}{I_{y}^*}\cdot z^*-\frac{M_{z}^*}{I_{z}^*}\cdot y^*$$

## Kroutivé napětí
#### Pro uzavřený profil
$$\large I_t=\frac{4\cdot A^{2}_t}{\Sigma\frac{h_i}{t_i}}$$
- TODO popsat co je co a dokreslit obrázky v excali

#### Pro otevřený profil
$$\large I_t = y\cdot \frac{1}{3}\cdot \Sigma h_i\cdot t^{3}_i$$
- TODO same
- 
## Kroutivé pootočení
$$\large \varphi = \frac{M_k\cdot l}{G\cdot I_t}\ \ \ \ [rad]$$
- $M_k$ - kroutivý moment ($KN\cdot m\; ; \; KPa)$
- $l$ - vzdálenost ($m$)
- $G$ - modul pružnosti ve smyku ($KPa$) - bude zadaný u oceli 81 $GPa$, takže dát $\cdot 10^6$
- $I_t$ - [[#Kroutivé napětí idk]] ($m^4$)
