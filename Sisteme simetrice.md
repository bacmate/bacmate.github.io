
## Sisteme de Ecuații Simetrice (Clasa a IX-a)

## 1. Definiție și Proprietăți

O ecuație $E(x, y) = 0$  se numește **simetrică** dacă forma ei nu se schimbă atunci când schimbăm variabilele între ele (înlocuim $x$ cu $y$ si $y$ cu $x$).

-   **Proprietate:** Dacă perechea $(\alpha, \beta)$ este soluție a sistemului, atunci și perechea "inversată" $(\beta, \alpha)$ este în mod obligatoriu soluție.
    

### Exemple (Sisteme algebrice simetrice):

-   $\begin{cases} x + y = 5 \\ x \cdot y = 6 \end{cases}$
    
-   $\begin{cases} x^2 + y^2 = 13 \\ x + y + xy = 11 \end{cases}$
    

### Contraexemple (Sisteme ne-simetrice):

-   $\begin{cases} x - y = 2 \\ x \cdot y = 3 \end{cases}$ (diferenta din prima ecuatie stric simetria!)
    
-   $\begin{cases} 2x + 3y = 12 \\ x^2 + y = 5 \end{cases}$ (coeficienții și exponenții diferiți strică simetria)
    

> **Rigurozitate matematică:** Metoda algebrică de rezolvare prin sumă ($s$) și produs ($p$) prezentată mai jos se aplică **exclusiv ecuațiilor polinomiale**. 

## 2. Sistemul Simetric Fundamental

Este sistemul în care se cunosc direct suma $s = x + y$ și produsul $p = x \cdot y$:

$$\begin{cases} x + y = s \\ x \cdot y = p \end{cases}$$

Conform" reciprocei" relatiilor Viète, $x$ și $y$ sunt rădăcinile ecuației de gradul al doilea:

$$t^2 - s \cdot t + p = 0$$

## 3. Metoda de rezolvare 

Orice sistem algebric simetric poate fi redus la variabilele $s = x + y$ și $p = x \cdot y$ folosind identitățile:

-   $x^2 + y^2 = s^2 - 2p$
    
-   $x^3 + y^3 = s^3 - 3sp$
    

### Model de rezolvare:

Să se rezolve în $\mathbb{R} \times \mathbb{R}$: $\begin{cases} x^2 + y^2 = 13 \\ x + y + xy = 11 \end{cases}$

1.  **Substituția:** Notăm $x+y=s$ și $xy=p$. Sistemul devine: $\begin{cases} s^2 - 2p = 13 \\ s + p = 11 \implies p = 11 - s \end{cases}$
    
2.  **Rezolvarea în $s$ și $p$:** Înlocuim $p$ în prima ecuație:
    
    $$s^2 - 2(11 - s) = 13 \implies s^2 + 2s - 35 = 0 \implies s_1 = 5, \, s_2 = -7$$
    
3.  **Determinarea lui $x$ și $y$ (Revenirea la substituție):**
    
    -   **Cazul I:** Pentru $s = 5 \implies p = 11 - 5 = 6$. Ecuația $t^2 - 5t + 6 = 0$ are rădăcinile $t_1 = 2, t_2 = 3$. Obținem soluțiile: **$(2, 3)$ și $(3, 2)$**.
        
    -   **Cazul II:** Pentru $s = -7 \implies p = 11 - (-7) = 18$. Ecuația $t^2 + 7t + 18 = 0$ are $\Delta = 49 - 72 < 0$ (nu are soluții reale).
        

-   **Soluția finală:** $S = \{(2, 3), (3, 2)\}$.
    

## 4. Temă pentru acasă 

Să se rezolve în $\mathbb{R} \times \mathbb{R}$ următoarele sisteme simetrice:

1.  $\begin{cases} x + y = 4 \\ x^2 + y^2 = 10 \end{cases}$
    
    _(Indiciu: Rezultă $s=4, p=3$. Soluții: $(1,3), (3,1)$)_
    
2.  $\begin{cases} x^2 + y^2 - xy = 7 \\ x + y = 5 \end{cases}$
    
    _(Indiciu: Rezultă $s=5, p=6$. Soluții: $(2,3), (3,2)$)_
    
3.  $\begin{cases} x^2y + xy^2 = 30 \\ x + y = 5 \end{cases}$
    
    
