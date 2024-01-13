# Lieární zobrazení na vektorových prostorech

## Lineární zobrazení

- Jsou-li _U_=(_M_, ⊕ᵤ, ⊗ᵤ), _V_=(_N_, ⊕ᵥ, ⊗ᵥ) vektorové prostory nad tělesem _T_ a _f_ zobrazení _M_ → _N_, řekneme, že zobrazení _f_ je lineární, pokud platí:
  - Aditivní zobrazení: **_f_(_u_ ⊕ᵤ _v_) = _f_(_u_) ⊕ᵥ _f_(_v_)**
  - Homogenní zobrazení: **_f_(α ⊗ᵤ _v_) = α ⊗ᵥ _f_(_u_)**
- Pokud je zobrazení současně aditivní a homogenní je lineární
- Lze zapsat do jedné podmínky
  - _f_((α ⊗ᵤ _u_) ⊕ᵤ (β ⊗ᵤ _v_)) = (α ⊗ᵥ _f_(_u_)) ⊕ᵥ (β ⊗ᵥ _f_(_v_))

### Známá lineární zobrazení

- Násobení matice*m*×*n* vektory z _T<sup>n</sup>_ je lineární zobrazení _T<sup>n</sup>_ → _T<sup>m</sup>_
- Přiřazení souřadnic v dané bazi k vektoru z _n_-rozměrného prostoru _V_ je lineární zobrazení _V_ → _Tⁿ_
  - I opačné přiřazení vektoru z _n_-rozměrného prostoru _V_ k souřadnicím v dané bazi je lineární zobrazení _Tⁿ_ → _V_
- Obecně každý izomorfismus dvojice vektorových prostorů _U_ a _V_ je lineární zobrazení _U_ → _V_ i _V_ → _U_
- Identita na libovolném vektorovém prostoru _V_ je lineární zobrazení _V_ → _V_
- Na prostoru orientovaných úseček v rovině jsou lineární zobrazení např. rotace o daný úhel, zkosení, projekce, ... (podobná existují i pro orientované úsečky v prostoru)

## Definiční obor lineárního zobrazení

- Je-li _U_=(_M_, ⊕ᵤ, ⊗ᵤ) a zobrazení _f_ : _U_ → _V_ lineární, pak (_D(f)_, ⊕ᵤ, ⊗ᵤ) je podprostor v _U_

## Obor hodnot lineárního zobrazení

- Je-li _V_=(_N_, ⊕ᵥ, ⊗ᵥ) a zobrazení _f_ : _U_ → _V_ lineární, pak (_W(f)_, ⊕ᵥ, ⊗ᵥ) je podprostor v _V_
- Hodností lineárního zobrazení _f_ : _U_ → _V_ nazýváme dimenzi jeho oboru hodnot
  - rank(_f_) = dim(_W(f)_)
- Pokud je zobrazení lineární => obrazem nulového vektoru je vždy nulový vektor
  - _f(oᵤ)_ = _f_(0 ⊗ᵤ _u_) = 0 ⊗ᵥ _f(u)_ = _oᵥ_

## Jádro lineárního zobrazení

- Je-li _U_=(_M_, ⊕ᵤ, ⊗ᵤ) a zobrazení _f_ : _U_ → _V_ lineární, nazveme množinu všech vektorů z _U_, jejichž obrazem je nulový vektor, jádrem lineárního zobrazení _f_
  - ker(_f_) = {_x_ ∈ _D(f)_ : _f(x)_ = _oᵥ_}
  - Jádro tohoto zobrazení je podprostorem v _U_ i v _D(f)_

## Linearita lineární kombinace

- Lineární kombinace lineárních zobrazení je lineární zobrazení (vše musí být nad stejným tělesem)

## Linearita složeného zobrazení

- Složené zobrazení lineárních zobrazení je lineární zobrazení

## Linearita inverzního zobrazení

- Inverzní zobrazení k prostému lineárnímu zobrazení je také lineární

## Zúžení lineárního zobrazení

- Je-li _f_ : _U_=(_M_, ⊕, ⊗) → _V_=(_N_, ⊕, ⊗) lineární zobrazení a _S_=(_L_, ⊕, ⊗) ⊂ _U_, nazýváme zobrazení _f_|_S_ : _S_ → _V_, kde
  - _D(f | S)_ = _L_ ∩ _D(f)_
  - _f | S(u)_ = _f(u)_ pro každé u ∈ \*D(f | S)
- Zúžením lineárního zobrazení na podprostor S, toto zůžení je znovu lineárním zobrazením

[Výpočetní náročnost operací s maticemi ⬅️](./07_NarocnostOperaciMatice.md) | [➡️ Frobeniova věta pro obecná lineární zobrazení](./09_FrobenioVeta.md)
