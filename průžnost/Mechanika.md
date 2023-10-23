# 1. Podklady pro výpočet
---
#### Beton C20/25
 - používá se první číslo
 - jednotka je **MPa**

## **$fcd = \frac{fck}{1,5}$**

#### Ocel B400B
-  $fyk$ se najde v tabulkách na straně **20**
-  většinou se používá číslo v názvu - **400**
-  jednotka je **MPa**


## **$fyd = \frac{fyk}{1,15}$**

# 2. Návrh rozměrů
---
#### Návrh výšky **$h$** a šířky **$b$**
- dá najít v tabulkách na straně 17 podle typu
#### Uložení **$u$**
- Konzolová, oboustranně vetknutá, s převislými konci - **nemá uložení**
- S převislým koncem, podestová deska - **$u=h$**
- Prostě uložený trám - $u$=7,5% z $ls$

# 3. Zatížení
----
## Stálé
- značí se $gd$
- zatížení od stropní kce, omítky, podlahy atd.
## **$gd=h*1.35*\rho$**

- $h$ je tloušťka konstrukce
## Nahodilé
- značí se $qd$
## **$qd=qk*1.5$**
- pokud není zadané $qk$, je v tabulkách na straně **12** - podle druhu účelu stavby
## Celkové
## **$fd=(gd+qd)*ZŠ$**
- ZŠ u desky - vždy 1
- ZŠ u trámu - osová vzdálenost trámů

# 4. Momenty
----

## **$M_{max}=Med=x*fd*l^2$**
## PRO **$x$**
#### Konzola  **$=-\frac{1}{2}$**
#### Oboustranně vetknutá deska
- dokonalé vetknutí
	- podpora $=-\frac{1}{12}$
	- pole $=\frac{1}{24}$
- částečné vetknutí
	- podpora $=-\frac{1}{16}$
	- pole $=\frac{1}{16}$
#### Podestová deska
- podpora $=-\frac{1}{8}$
- pole $=\frac{1}{10}$
#### Prostě uložený trám
- pole $=\frac{1}{8}$
---
#### Deska s převislými konci nebo koncem
## **$Med_{podpora}=-\frac{1}{2}*fd*l_1^2$**
## **$Med_{pole}=-\frac{1}{2}*gd*l_1^2+\frac{1}{8}*fd*l_2^2$**
- $l_1$ je délka převislého konce (balkonu)
- $l_2$ je délka stropní desky uvnitř
# 5. Návrh výztuže
---
- musíme navrhnout předpoklad průměru hlavní výztuže $⌀_{hl}$ (14mm) a krytí $c$ (25mm)
#### Staticky účinná výška **$d$**
##### Pro desku:
## **$d=h-c-\frac{⌀_{hl}}{2}$**
##### Pro trám:
## **$d=h-c-⌀_{třm}\frac{⌀_{hl}}{2}$**
## Návrh hlavní výztuže
#### Minimální plocha výztuže
## **$As_{min} = b*d*\frac{fcd}{fyd}*\left( 1-\sqrt{1-\frac{2*Med}{b*d^{2}*fcd}} \right)$** 
- doporučuji zadávat jednotky v [mm, N, MPa] - výsledek posunout o 6 desetinných míst
- podle výsledku vybrat výztuž z tabulek strana **21 - trám**, **22 - desky** (lepší předimenzovat o 10%)
- výsledkem je $As$ ve tvaru $⌀$ 14 po 250mm ( $As=616 mm^2/m$ )
## Návrh třmínků ( trám )
## **$⌀tř=\frac{1}{4}*⌀_{hl}$**
- min. průměr je 6mm
## Návrh rozdělovací výztuže ( desky )
## **$As_{r,min}=0.2*As$**
- návrh z tabulek strana **22**
- min. průměr je 6mm
# 6. Návrh krytí
---
### Deska
## **$c_{min}=max \{⌀_{hl};c_{min,dur};10\}$** 
- $c_{min,dur}$ - vliv prostředí - tabulky strana **14**
- pokud není zadáno tak $c_{min,dur}=15$
## **$c_{nom}=c_{min}+c_{\Delta def}$** 
- $c_{\Delta def}$ - u monolitických konstrukcí (v našem případě **vždy**) **10mm**
## **$c\ge c_{nom}$** 

**Výsledkem je krytí $c$**

### Trám
- počítá se zvlášť krytí pro hlavní výztuž a třmínek, a poté se **vybere větší** z  těchto hodnot
- výpočet krytí $hl$ **stejné jako u desky**
- výpočet krytí třmínku se vypočítá stejně jako u $hl$, pouze s jiným průměrem výztuže ($⌀_{třm}$) a poté se k výslednému krytí přičte $⌀_{třm}$ a výsledná hodnota se porovná s krytím $hl$ --> vybere se větší z hodnot

# 7. Posouzení
---
#### 1. **POUZE PRO TRÁM** Posouzení, jestli se výztuž do průřezu vejde...
## **$a_{min}=max\{1.2*⌀_{hl};dg+5;20\}$**
- $a_{min}$ - mezera mezi jednotlivými pruty $hl$
- $dg$ - velikost největší frakce kameniva - v našem případě vždy **16**

## **$b_{w,min}=2*c+2*⌀_{třm}+n*⌀_{hl}+(n-1)*a_{min}$**
- $n$ - počet navržených prutů $hl$ v trámu
	- př. 4 $⌀$ 14 ( $As=616 mm^2/m$ ) --> $n=4$ 

## **$b_{w,min}\le b$**              ✔
### 2. Výška tlačené části **$x$**

## **$x=\frac{As * fyd}{0.8*b*fcd}$** 
- doporučuji zadávat jednotky v [mm, N, MPa]
- u desky $b=1000mm$
### 3. Moment
- Musíme přepočítat staticky účinnou výšku $d$
# **$d=h-c-\frac{⌀_{hl}}{2}$**
- Spočítáme $Mrd$ - (musí být větší než $Med$)
## **$Mrd=As*fyd*(d-0.4*x)$**
## **$Med\le Mrd$**               ✔
### 4. Poměr tlačené části **$\xi$**
## **$\xi=\frac{x}{d}$** 
## **$\xi \lt 0.45$**               ✔
### 5. Stupeň vyztužení
## **$\rho = \frac{As}{Ac} = \frac{As}{b*d}$**
## **$\rho _{min} \lt \rho \lt \rho _{max}$**              ✔
- $\rho _{min}$ a $\rho _{max}$ se najde v tabulkách na straně **18**
- pro desky i trámy:
	- $\rho _{min}=0.0013$
	- $\rho _{max}=0.04$

# 8. Návrh kotevní délky
---
## **$l_{bd}=\alpha * ⌀_{hl}$**
- $\alpha$ - součinitel pro výpočet základní kotevní délky
	- dá se najít na straně **16**
### Návrh **$\Delta l$**
## **$\Delta l=max\{0.3*l_{bd};10*⌀_{hl};100\}$**
- zpravidla vychází největší $0.3*l_{bd}$