# Číselné matice a Operace s nimi

## Násobení matic

- Matici _m<sub>1</sub>×n<sub>1</sub>_ můžeme vynásobit maticí _m<sub>2</sub>×n<sub>2</sub>_ pokud _n<sub>1</sub>_ = _m<sub>2</sub>_
  - Rozměr výsledné matice je _m<sub>1</sub>×n<sub>2</sub>_
- Násobení matic je komutativní
- Násobení matic je asociativní
- Řádek v*i*-tém řádku a _j_-tém sloupci lze chápat jako součet součinů prvků _i_-tého řádku první matice s _j_-tým sloupcem druhé matice

## Matice přechodu

- Sloupce matice _P<sub>E→F</sub>_ jsou tvořeny souřadnicovými vektory vektorů baze _E_ v bazi _F_
- Vynásobením _P<sub>E→F</sub>_ vektorem se souřadnicemi v bazi _E_ dostaneme jeho souřadnice v bazi _F_
- _P<sub>E→G</sub>_ = _P<sub>F→G</sub>_ ⋅ _P<sub>E→F</sub>_
  - Jdeme zprava do leva

### Konstrukce matice přechodu

- (_Y_ | _X_) ~ (_I_ | _P<sub>X→Y</sub>_) ~ (_P<sub>Y→X</sub>_ | _I_)
- Do levé části matice vepíšeme (po sloupcích ve správném pořadí) vektory cílové baze a do pravé části vektory startovní baze
  - Po použití Gauss-Jordanovy eliminační metody nám vlevo vyjde jednotková matice a v pravo vyjde matice přechodu
- Pro přechod z baze do kanonické baze stačí vepsat bazové vektory (nekanonické) baze po sloupcích do matice

## Matice reprezentující gaussovské operace

- Gaussovské operace s řádky matice se dají chápat jako násobení eliminované matice speciální "gaussovskou" maticí _G_ **zleva**

1. Výměna řádků _i_, _j_
   1. Matice G jhe stejná jako jednotková matice, jenmá prohozené řádky _i_ a _j_
   2. g<sub>_ij_</sub> = g<sub>_ji_</sub> = 1
   3. g<sub>_kk_</sub> 1 pro všechna _k_ kromě _k_ = _i_ a _k_ = _j_
2. Vynásobení _i_-tého řádku číslem _a_
   1. Matice G je stejná jako jednotková matice, na řádku _i_ je ale místo jedničky číslo _a_
   2. g<sub>_kk_</sub> = 1 pro všechna _k_ kromě _k_ = _i_
   3. g<sub>_ii_</sub> = _a_
3. Přičtení _a_-násobku _i_-tého řádku k _j_-tému řádku
   1. g<sub>_ji_</sub> = _a_
   2. g<sub>_kk_</sub> = 1
4. Vynechání _i_-tého řádku
   1. G je matice s _n_-1 řádky a _n_ sloupci
   2. g<sub>_k,k_</sub> = 1 pro všechna _k_ < _i_
   3. g<sub>_k,k_+1</sub> = 1 pro všechna _k_ ≥ _i_

## Jednotková matice

- Existuje právě jedna
- Na diagonále má jedničky a všude jinde nuly

## Inverzní matice

- Matice _P<sub>F→E</sub>_ = (_P<sub>E→F</sub>_)<sup>-1</sup>
- K regulárním maticím lze vytvořit inverzní matici, k singulárním nikoli
- Výpočet
  - Do levé části napíšeme půvdní matici, do pravé jednotkovou matici.
  - Provedeme Gaussovu-jordanovu eliminaci => vlevo nám vyjde jednotková matice v pravo inverzní matice
  - S jednotkovou matici provádíme pouze operace, které provádíme při transformaci původní matice na jednotkovou

## Matice jako uspořádaná sada čísel

- Číselná matice *m*×*n* je uspořádanou _mn_-ticí čísel, lze ji považovat za vektor z _T<sup>m×n</sup>_
- Součet matic _A_ a _B_ o rozměrech *m*×*n* je matice _C_ = _A_ + _B_, která má také rozměr *m*×*n* a platí _c<sub>ij</sub>_ = _a<sub>ij</sub>_ + _b<sub>ij</sub>_
- α-násobkem matice _A_ je matice _C_ = α*A* o stejných rozměrech, kde platí _c<sub>ij</sub>_ = α*a<sub>ij</sub>*
- Tímto způsobem můžeme také zavést lineární kombinaci
- Kromě toho, že násobení matic není komutativní, můžeme s maticemi při kombinování sčítání a násobení (další maticí nebo číslem) zacházet stejně jako s čísly

## Transpozice matice

- Vzájemná výměna řádků a sloupců

## Bloková matice

- Matici můžeme vodorovnými a svislými čarami rozdělit na části nazývané bloky, což jsou opět matice obecně menších rozměrů
- Bloková matice _A_ *m*×*n*, jejímiž prvky jsou matice _A<sub>ij</sub>_ navzájem kompatibilních rozměrů *r<sub>i</sub>*×*s<sub>j</sub>*
- Na blokové matice lze pohlížet jako na běžné matice
- Jsou-li ovšem sčítané/násobené matice rozděleny do bloků "sobě odpovídajícím způsobem", pak jejich součet/násobek lze opět zapsat jako blokovou matici a operace sčítání/násobení je možné provádět po blocích

[Lineární závislost vektorů ⬅️](./05_LinearniZavislostVektoru.md) | [➡️ Výpočetní náročnost s maticemi](./07_NarocnostOperaciMatice.md)
