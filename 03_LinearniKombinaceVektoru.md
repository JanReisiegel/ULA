# Lineární kombinace vektorů

## Lineární kombinace vektorů

- _b_ = α₁ ⊗ _a₁_ ⊕ α₂ ⊗ _a₂_ ⊕ · · · ⊕ αₙ ⊗ _aₙ_
- Vektor _b_ je lineární kombinací vektorů _a₁_, _a₂_, ..., _aₙ_ s koeficienty α₁, α₂, ..., αₙ → je součtem jejich násobků
- Pro _V_ = (_M_, ⊕, ⊗) nad tělesem _T_, kde _a_ ∈ _M_ a α ∈ _T_

## Lineární obal množiny vektorů

- Je-li _A_ = {_a₁_, _a₂_, ..., _aₙ_(, ...)} množina vektorů z _M_ a _V_ = (_M_, ⊕, ⊗) vektorový prostor nad tělesem _T_, nazveme množinu všech lineárních kombinací vektorů _a<sub>i</sub>_ **lineárním obalem** množiny _A_ Lineární obal množiny _A_ značíme span(_A_)

1. Pokud vynásobíme vektor z množiny _A_ nenulovým číslem, span(_A_) se nezmění
2. Obal se také nezmění, pokud k jednomu vektoru přičteme libovolný násobek **jiného** vektoru
3. Obal se také nezmění, pokud vynecháme vektor, který je lineární kombinací **ostatních** vektorů (takový vektor můžeme také přidat)

- Je-li _A_ = {_a₁_, _a₂_, ..., _aₙ_, ...} množina vektorů z _M_ a _V_ = (_M_, ⊕, ⊗) vektorový prostor nad tělesem _T_, pak trojice (span(_A_), ⊕, ⊗) je **podprostorem** ve _V_
  - Říkáme, že množina A generuje podprostor (span(_A_), ⊕, ⊗)

## Gausova eliminační metoda

- Z každé matice lze vytvořit matici v horním stupňovitém tvaru pomocí posloupnosti gaussovských operací
  1. Výměna řádků
  2. Nenulové vynásobení řádku
  3. Přičtení násobku jiného řádku
- Gaussova eliminační metoda spočívá v opakování postupu, kdy se v aktuálně zpracovávané submatici snažíme pomocí gaussovských operací vytvořit v prvním sloupci nuly na všech místech nejvýše s vyjímkou prvního řádku submatice

[Vektorový prostor ⬅️](./02_VektorovyProstor.md) | [➡️ Soustavy lineárních rovnic](./04_SoustavyLinearnichRovnic.md)
