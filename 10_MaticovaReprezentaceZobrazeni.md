# Maticová reprezentace lineárního zobrazení

- Cíl: najít souřadnice vektoru _f(u)_ v bazi _F_, pokud známe souřadnice _u_ v bazi _E_
  - Zjistit zda vůbec obraz _f(u)_ existuje, může být problémové
  - Problému se lze vyhnout, pokud se budeme zabývat zobrazením _f|D(f)_ : _Ũ_(_D(f)_, ⊕ᵤ, ⊗ᵤ) → _V_ (zúžení na definiční obor)
- Matice _P<sub>E→F</sub>_ se nazývá maticová reprezentace lineárního zobrazení _f_ v bázích _E_ a _F_
  - rozměry jsou dim(_V_)×dim(_U_) (dimenze prostoru obrazů×dimenze prostoruvzorů)
- Pokud:
  - U=(M, ⊕ᵤ, ⊗ᵤ) a V=(N, ⊕ᵥ, ⊗ᵥ) jsou konečnorozměrné prostory
  - E ⊂ M a F ⊂ N jsou baze těchto prostorů
  - Zobrazení f : U → V je lineární
  - D(f) = M
- pak existuje taková matice F<sub>E→F</sub>, že (f(u))<sup>F</sup> = F<sub>E→F</sub> ⋅ uᴱ pro každý vektor u ∈ M
  - tato matice je určena jednoznačně
  - Pro vytvoření matice F<sub>E→F</sub> najdeme obrazy f(e<sub>j</sub>) všech bazových bektorů baze E a určíme jejich souřadnice v bazi F, ty ve správném pořadí zapíšeme po sloupcích do matice

## Hodnost matice

- Obor hodnot lineárního zobrazení tvoří podprostor v cílové množině, nazývá se hodnost zobrazení
  - rank(f) = dim(W(f))
- Každý vektor z W(f) je lineární kombinací vektorů f(e<sub>j</sub>)
- Počet lineárně nezávislých sloupců/řádků matice se nazývá hodnost matice

## Maticové reprezentace operací

- Maticovou reprezentaci identity ve stejných bazích je jednotková matice
  - Identita v různých bazích je pak matice přechodu
- Maticová reprezentace složeného lineárního zobrazení je lineární kombinací maticových reprezentací původních zobrazení (ve stejných bazích se stejnými koeficienty)
- Maticová reprezentace složeného lineárního zobrazení je součinem maticových reprezentací jednotlivých zobrazení
- Maticová reprezentace případného inverzního lineárního zobrazení je rovna inverzní matici reprezentující původní lineární zobrazení (v příslušných bazích obou prostorů)

[Frobeniova věta ⬅️](./09_FrobenioVeta.md) | [➡️ Zobrazení prostoru do sebe](./11_ZobrazeniProstoruDoSebe.md)
