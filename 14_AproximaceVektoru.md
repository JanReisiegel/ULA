# Aproximace vektoru

## Aproximace

- nepotřebujeme skoro nikdy znát vektory úplně přesně, můžeme uvažovaný vektor nahradit jiným, kterýá je k němu dostatečně blízko a práce s ním je jednodušší
- Na prostorech se skalárním součinem je zavedena velikost vektoru => můžeme přesně definovat "dostatečně blízko"
  - uvažovaný vektor _u_ se od náhradního vektoru _u<sub>V</sub>_ liší o velmi malý vektor _u_ = *u<sub>v</sub> ⊕ *δ<sub>u</sub>*, ||*δ<sub>u</sub>*||≤dané *ε\*
  - Náhradní vektor _u<sub>V</sub>_ hledáme zpravidla v nějakém konečněrozměrném prostoru _V_ daného prostoru _U_
- Předpokládejme *V*⊂*U*, ve kterém hledáme _u<sub>v</sub>_, je pevně daný
- nejlepší přiblížení _u_ z prostoru _U_ vektorem z _V_ bude takový vektor _u<sub>V</sub>_, který bude splňovat: **||_u_ ⊕ (-_u<sub>v</sub>_)||≤||_u_ ⊕ (-_v_)||** pro ∀ _v_ ∈ _V_
- Označíme _δ<sub>u</sub>_ = _u_ ⊕ (-_u<sub>V</sub>_), a protože vektorry _u<sub>V</sub>_ i _v_ jsou v prostoru _V_ existuje _w_ ∈ _V_ tak, že _u<sub>V</sub>_ = _v_ ⊕ _w_
- Požadavek optimality: ||_δ<sub>u</sub>_|| ≤ ||_u_ ⊕ (-_u<sub>V</sub>_) ⊕ _u<sub>V</sub>_ ⊕ (-_v_)|| = ||_δ<sub>u</sub>_ ⊕ _w_|| pro každý vektor _w_ z prostoru _V_

### Vlastnost odchylky

- Podmíka optimality je nerovnost mezi dvěma nezápornými čísly
- umocníme podmínku optimality na druhou a dostamene:
  - ||_δ<sub>u</sub>_||<sup>2</sup> ≤ ||_δ<sub>u</sub>_ ⊕ _w_||<sup>2</sup> = ⟨_δ<sub>u</sub>_ ⊕ _w_|_δ<sub>u</sub>_ ⊕ _w_⟩ = ⟨_δ<sub>u</sub>_|_δ<sub>u</sub>_⟩ + ⟨_δ<sub>u</sub>_|_w_⟩ + ⟨_w_|_δ<sub>u</sub>_⟩ + ⟨_w_|_w_⟩
  - 0 = ⟨_δ<sub>u</sub>_|_w_⟩ + ⟨_w_|_δ<sub>u</sub>_⟩ + ⟨_w_|_w_⟩
- Tento vztah musíplatit pro každý nenulový vektor _w_ z podprostoru _V_ (pro _w_ = _o_ platí triviálně), tedy i pro vektor w' = -⟨_w_|_δ<sub>u</sub>_⟩/||_w_||<sup>2</sup> ⊗ _w_
  - ![Vlastnost odchylky](pic/aproximace1.png)
- Má-li být splněna podmínka 0 ≤ - |⟨_w_|_δ<sub>u</sub>_⟩|<sup>2</sup>/||_w_||<sup>2</sup> pro všechny _w_ z _V_ musí být ⟨_w_|_δ<sub>u</sub>_⟩ = 0

  - tedy _δ<sub>u</sub>_ musí být kolmý na všechny vektory z prostoru _V_
  - ![Nejlepší přiblížení](pic/aproximace2.png)
  - Hledané nejlepší přiblížení vektoru _u_ vektorem _u<sub>V</sub>_ z prostroru _V_ proto také charakterizujeme jako kolmý průnět vektoru _u_ so prostoru _V_.

- Je-li _U_ vektortový prostor se skalárním součinem, _V_ ⊂ _U_ jeho úplný podprostor a vektor _u_ ∈ _U_, pak existuje právě jeden vektor _u<sub>V</sub>_ ∈ _V_ takový, že ||_u_ ⊕ (-_u<sub>V</sub>_)|| ≤ ||_u_ ⊕ (-_v_)|| pro všechny _v_ ∈ _V_
- Pokud najdeme jeden vektor _u<sub>V</sub>_ takový, že optimálně aproximuje vektor _u_ na podprostoru _V_, můžeme pro libovolný vektor _v_ ∈ _V_ vyjádřit vektor _u<sub>V</sub>_ jako součet *u<sub>V</sub> = *v* ⊕ *w* pro nějaké *w* ∈ *V\*
- ![Alt text](pic/aproximace3.png)
- a protože _u<sub>V</sub>_ je ⟨_w_|_δ<sub>u</sub>_⟩ = 0 pro všechny vektory _w_ z podprostoru _V_ je
- ![Alt text](pic/aproximace4.png)
- pro všechny _w_ ≠ _o_, a tedy nalezené optimální přiblížení je jediné

Pokud je podprostor _V_ konečněrozměrný, můžeme v něm najít bazi _G_ = {**g**<sub>j</sub>}<sub>j=1</sub><sup>n</sup> a hledaný vektor _u<sub>V</sub>_ popsat jeho souřadnicemi _u<sub>j</sub>_ v této bazi

![Vektor uv](pic/aproximace5.png)

![Podmínka optimality](pic/aproximace6.png)

- pro všechny vektory _w_ ∈ _V_ musí platit speciálně i pro vektory _w_ = **g**<sub>_i_</sub> ∈ _V_ tedy

![Alt text](pic/aproximace7.png)

- pro všechny vektory **g**<sub>_i_</sub> ∈ _G_

## Soustava rovnic a přímý výpočet

![Soustava rovnic](pic/aproximace8.png)

- soustava _n_ rovnic pro _n_ neznámých součadnic _u<sub>j</sub>_ s metrickou maticí **G** generovanou množinou _G_
- Je-li baze _G_ ortogonální jsou všechny prvky matice **G** s vyjímkou těch diagonálních nulové, a vyjde

![Alt text](pic/aproximace9.png)

- kdyby existovala ortogonální bsze celého _U_ a _V_ by byl lineárním obalem jejích prvních _n_ vektorů, dostaneme hledané optimální přiblížení pomocí prvních _n_ souřadnic vektoru _u_ v bazi _G_

### výpočet velikosti aproximace

- známe-li už souřadnice _u<sub>i</sub>_ hledaného přiblížení v bazi _G_, známe i toto přiblížení a můžeme spočítat
- ![Alt text](pic/aproximace10.png)
- což je druhá mocnina normy souřadnicového vektoru **u**<sup>(_g_)</sup> při skalárním součinu s metrikou **G**
- V případě, že je baze _G_ podprostoru _V_ ortogonální, můžeme souřadnice _u<sub>j</sub>_ spočítat přímo a
- ![Alt text](pic/aproximace11.png)

### Rozšiřování aproximačnéího podprostoru
- Uvažujme posloupnost vektorů (_a<sub>i</sub>_)<sub>*i*≥1</sub> z unitárního prostoru _U_ a posloupnost podprostotů _V<sub>j</sub>_ = span{_a<sub>i</sub>_}<sub>_i_=1</sub><sup>j</sup>
  - Pro každé přirozené j < (počet vektorů v posloupnosti (*a<sub>u</sub>)) je *V<sub>j</sub>* ⊂ *V*<sub>*j*+1</sub>
  - Z posloupnosti (*a<sub>i</sub>*) odstraníme všechny vektory které jsou leneárními kombinacemi předcházejících členů této posloupnosti, dostaneme tak lineárně nezávislou množinu *A'*={*a'<sub>i</sub>*}<sub>*i*≥1</sub> a odpovídající posloupnost podprostorů *V'<sub>j</sub>* = span{*a'<sub>i</sub>*}<sub>*i*≥1</sub><sup>j</sup>
  - Ortogonalizací množiny *A'* dostaneme ortogonální množinu *G*={**g**<sub>*i*</sub>}<sub>*i*≥1</sub>
    - Každá množina *G*<sub>*j*</sub> = {**g**<sub>*i*</sub>}<sub>*i*≥1</sub><sup>j</sup> bude ortogonální bazí odpovídajícího podprostoru *V'<sub>j</sub>*

### Pokles velikosti chyby
![Pokles velikosti chyby](pic/aproximace12.png)
- rozšiřováním aproximačního podprostoru *V* se aproximace vektoru *u* zpravidla zlepšují, nikdy se nemohou zhoršit

## Metoda nejmenších čtverců
