

# Fișă Auxiliară:  (Limite și Integrale )

---

## I. LIMITE (Subiectul al III-lea, ex. 1)
$$\boxed{\lim_{x \to \pm\infty} \frac{ax + b}{cx + d} = \frac{a}{c}}$$

### 1. Limite cu Radicali și Capcana de la $-\infty$ (Foarte Important!)
Când  avem fractie cu radicali:
* **Cazul $x \to \infty$:** 
    $$\lim_{x \to \infty} \frac{x}{\sqrt{x^2+a}} = 1$$
* **Cazul $x \to -\infty$ (Atenție la semn! ⚠️):** Ieșirea lui $x$ de sub radicalul de ordin par generează $|x| = -x$.
    $$\lim_{x \to -\infty} \frac{x}{\sqrt{x^2+a}} = -1$$
    Pentru diferente de radicali in cazul $\infty-\infty$ se amplifica cu conjugata:
    $$\lim_{x \to \infty} (\sqrt{x^2+x} - x) = \lim_{x \to \infty} \frac{(\sqrt{x^2+x} - x)(\sqrt{x^2+x} + x)}{\sqrt{x^2+x} + x} = \lim_{x \to \infty} \frac{(x^2+x) - x^2}{\sqrt{x^2+x} + x} = \lim_{x \to \infty} \frac{x}{x\left(\sqrt{1+\frac{1}{x}} + 1\right)} = \frac{1}{1+1} = \frac{1}{2}$$
    NOTA: Nu aplicati conjugata "din reflex", daca nu e caz de nedeterminare:
    $$\lim_{x \to -\infty} (\sqrt{x^2+x} - x) = \sqrt{(-\infty)^2} - (-\infty) = \infty + \infty = \infty$$
    A iesit direct (observatie: sub radical fiind un polinom, conteaza doar termenul cu $x^2!)$

### 2. Limite cu Logaritmi ($\ln$)
* **Proprietatea diferenței (transformare în raport):**
    $$\lim_{x \to \infty} \left[ \ln(x+a) - \ln(x+b) \right] = \lim_{x \to \infty} \ln\left(\frac{x+a}{x+b}\right) = \ln(1) = 0$$
* **Limite standard:**
    $$\boxed{\ln(\infty) = \infty \quad \text{și} \quad \ln(0_+) = -\infty}$$
* **Șabloane rapide bazate pe dominanță (Logaritm contra Polinom):**
    * Puterea(sau polinomul) domină logaritmul la $\infty$:
        $$\boxed{\lim_{x \to \infty} \frac{ \ln x}{x^n} = 0, n>0}$$
    * 
        $$\lim_{x \to 0_+} \frac{\ln x}{x} = \frac{-\infty}{0_+} = -\infty$$

### 3. Limite cu Exponențiale ($e^x$)
* **Limite standard:**
    $$\boxed{e^\infty = \infty \quad \text{și} \quad e^{-\infty} = 0}$$
* **Șabloane rapide :**
    * Exponențiala domină polinomul și logaritmul la $\infty$:
    * $$\boxed{\lim_{x \to \infty} \frac{x^n}{e^x} = 0, \quad \forall n \in \mathbb{N}^*}$$
    *   $$\lim_{x \to \infty} (x - \ln x) = \infty \quad \text{și} \quad \lim_{x \to \infty} (e^x - x) = \infty$$
    * Raport de exponențiale similare:
        $$\lim_{x \to \infty} \frac{e^x}{e^x + a} = 1$$
    * Produse cu exponențială la $\infty$ și $-\infty$ (Cazul Nedeterminat $0 \cdot \infty$ rezolvat):
        $$\lim_{x \to \infty} x e^{-x} = \lim_{x \to \infty} \frac{x}{e^x} = 0$$
        $$\lim_{x \to -\infty} x e^x = \lim_{x \to -\infty} \frac{x}{e^{-x}} \left[\frac{-\infty}{\infty}\right] \stackrel{\text{l'H}}{=} \lim_{x \to -\infty} \frac{(x)'}{(e^{-x})'} = \lim_{x \to -\infty} \frac{1}{-e^{-x}} = \frac{1}{-\infty} = 0$$
        DAR:
        $$\lim_{x \to -\infty} x e^{-x} = (-\infty) \cdot e^{\infty} = -\infty$$
        Alt exemplu:
        $$\lim_{x \to -\infty} e^x(2x - 4) = 0 \quad \text{(prin l'Hospital ptr } \frac{2x-4}{e^{-x}}\text{)}$$
    * Scrierea lui x ca un logaritm:
        $$\lim_{x \to \infty} \left[ x - \ln(e^x + \dots) \right] = \lim_{x \to \infty} \left[ \ln(e^x) - \ln(e^x + \dots) \right]=\ln1=0$$
        Alt exemplu:
        $$\lim_{x \to \infty} \frac{e^{-x}}{x + 1} = \frac{0}{\infty} = 0$$

### 4. Cazurile de nedeterminare cu puteri
### Cazul $1^\infty$ (Scurtătura directă)
Avem limitele standard:
$$\lim\limits_{x \to \infty} \left(1 + \frac{1}{x}\right)^x = e$$ si $$\lim\limits_{x \to 0} (1 + x)^{\frac{1}{x}} = e$$
Când ai o limită de forma $\lim\limits_{x \to x_0} [f(x)]^{g(x)}$ unde $f(x) \to 1$ și $g(x) \to \infty$, aplici direct formula rapidă bazată pe limita fundamentală a numărului $e$:

$\boxed{\lim\limits_{x \to x_0} [f(x)]^{g(x)} = e^{\lim\limits_{x \to x_0} (f(x) - 1) \cdot g(x)}}$
### Cazurile $0^0$ și $\infty^0$ (Metoda logaritmării)
Metoda consta in  trecerea la baza $e$:

$$\boxed{[f(x)]^{g(x)} = e^{g(x) \ln f(x)}}$$

Prin această transformare, nedeterminarea inițială ($0^0$ sau $\infty^0$) se transformă întotdeauna într-un caz de tipul **$0 \cdot \infty$**, unde folosim metoda standard, scriind: 
$$f \cdot g = \frac{f}{\frac{1}{g}}$$ sau 
$$f \cdot g = \frac{g}{\frac{1}{f}}$$
pentru aplicarea regulii L'Hospital.


## II. INTEGRALE (Subiectul al III-lea, ex. 2)
$$\boxed{\int \sqrt{x} \, dx = \frac{2}{3}x\sqrt{x} + \mathcal{C}}$$
$$\boxed{\int \frac{1}{\sqrt{x}} \, dx = 2\sqrt{x} + \mathcal{C}}$$

### 1. Tipuri cu Schimbare de Variabilă Directă / Formule Compuse
* **Tipul $\frac{u'(x)}{u(x)}$ (Logaritm):**
    $$\boxed{\int \frac{u'(x)}{u(x)} \, dx = \ln|u(x)| + \mathcal{C}}$$
    * **Exemple:**
    * $$\boxed{\int \frac{1}{x+a} \, dx = \ln|x+a| + \mathcal{C}}$$
   
    * $$\int \frac{1}{ax+b} \, dx = \frac{1}{a}\ln|ax+b| + \mathcal{C}$$
     * $$\int_0^1 \frac{2x+2}{x^2+2x+5} \, dx = \left. \ln(x^2+2x+5) \right|_0^1 = \ln(8) - \ln(5) = \ln\left(\frac{8}{5}\right)$$
     * $$\boxed{\int \frac{x}{x^2 + a^2} \, dx = \frac{1}{2} \ln(x^2 + a^2) + \mathcal{C}}$$
     * $$\int \frac{x^2}{x^3+1} \, dx = \frac{1}{3} \int \frac{3x^2}{x^3+1} \, dx = \frac{1}{3} \ln|x^3+1| + \mathcal{C}$$
    * **Exemplu cu exponențială:**
        $$\int \frac{e^x}{e^x \pm a} \, dx = \ln(e^x \pm a) + \mathcal{C}$$
        Un alt tip des intalnit:
        $$\boxed{\int u(x) \cdot u'(x) \, dx = \frac{u^2(x)}{2} + \mathcal{C}}$$
*Exemplu:* $$\int \frac{\ln x}{x} \, dx = \frac{1}{2}\ln^2(x) + \mathcal{C}$$
*  ### 2. Integrale cu Radicali (Forme care conțin $x^2 + a$) 
*  **Forma cu $x$ la numărător :**   $$\boxed{\int \frac{x}{\sqrt{x^2+a^2}} \, dx = \sqrt{x^2+a^2} + \mathcal{C}}$$ 
$$\int \frac{x}{\sqrt{a^2-x^2}} \, dx  = -\sqrt{a^2-x^2} + \mathcal{C}$$**Forma cu radicalul înmulțit cu $x$:** $$\int x\sqrt{x^2+a^2} \, dx = \frac{1}{3}(x^2+a^2)\sqrt{x^2+a^2} + \mathcal{C}$$ 

* ### 3. Integrale rezolvate prin Părți (Forme Standard des intalnite) * 
* **Proprietate utilă de reținut pentru simplificare:** $$\ln(e^x) = x \quad \text{și} \quad e^{\ln x} = x$$ * **Polinom $\times$ Exponențială:** $$\boxed{\int x e^x \, dx = (x - 1)e^x + \mathcal{C}}$$ $$\int x e^{-x} \, dx = -e^{-x}(x + 1) + \mathcal{C}$$ * **Polinom $\times$ Logaritm:** $$\boxed{\int \ln x \, dx = x \ln x - x + \mathcal{C}}$$ $$\int x \ln x \, dx = \frac{x^2}{2}\ln x - \frac{x^2}{4} + \mathcal{C}$$ 
$$\int \frac{\ln x}{x^2} \, dx = -\frac{\ln x}{x} - \frac{1}{x} + \mathcal{C} = -\frac{\ln x + 1}{x} + \mathcal{C}$$
* ### 4. Tipul special prin artificiu de calcul (Adunare și Scădere la numărător) 
 * Pentru integrale de tipul $\int \frac{x}{x+1} \, dx$, se adună și se scade $1$ la numărător pentru desfacerea în două fracții: $$\int \frac{x}{x+1} \, dx = \int \frac{x+1-1}{x+1} \, dx = \int \left(1 - \frac{1}{x+1}\right) \, dx = x - \ln|x+1| + \mathcal{C}$$
 * $$\int \frac{1}{e^x+1} \, dx = \int \frac{1 + e^x - e^x}{e^x+1} \, dx = \int \left(\frac{e^x+1}{e^x+1} - \frac{e^x}{e^x+1}\right) \, dx = \int 1 \, dx - \int \frac{e^x}{e^x+1} \, dx = x - \ln(e^x+1) + \mathcal{C}$$
