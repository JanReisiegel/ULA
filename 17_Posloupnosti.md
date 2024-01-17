# Posloupnosti

Posloupnost (**a**) = (_a_<sub>1</sub>, _a_<sub>2</sub>, ... _a_<sub>n</sub>[,...]) je zobrazení z množiny přirozených čísel do dané množiny _M_. Prvek _a_<sub>j</sub> ∈ _M_ je obrazem čísla _j_ ∈ _N_ a nazýváme ho _j_-tým členem posloupnosti.

- vyžadujeme, aby nebyly díry => s každým číslem _n_ ∈ _N_ posloupnost obsahovala i _n_ - 1 (pokud _n_ ≠ 1)
  - _D_(**a**) = {1, 2, ..., _n_} - konečná _n_-prvková posloupnost
    - _n_-prvkové číselné posloupnosti jsou uspořádané _n_-tice čísel z dané množiny _M_
    - pokud je množina _M_ tělesem, jsou _n_-prvkové číselné posloupnosti vektory v _M<sup>n</sup>_
  - _D_(**a**) = _N_ - nekonečná posloupnost
    - očekáváme, že budeme schopni určit jakýkoli _n_-tý člen \*a<sub>n</sub>
      - nalezení přímého vztahu: _a<sub>n</sub>_ = _f_(_n_) - explicitně výjádřený člen
    - O posloupnosti (_a<sub>i</sub>_)<sub>*i*≥1</sub> řekneme, že je definovaná rekurentně, pokud _a<sub>k</sub>_ = _f_(_k_, _a_<sub>1</sub>, _a_<sub>2</sub>, . . . , _a_<sub>*k*−1</sub>) pro každé _k_ > _n_<sub>0</sub>. Konečnou část posloupnosti (_a<sub>i</sub>_)<sub>_i_=1</sub><sup>_n_<sub>0</sub></sup>, pro kterou platnost neočekáváme, pak můžeme definovat výčtem hodnot _a_<sub>1</sub>, _a_<sub>2</sub>, ..., _a_<sub>_n_<sub>0</sub></sub>. => počáteční podmínky
      - (**a**): _a<sub>j</sub>_ = 1 => rekurentně:<br> _a_<sub>1</sub> = 1, _a<sub>n</sub>_ = _a_<sub>_n_-1</sub> pro _n_ > 1
      - (**a**): _a<sub>n</sub>_ = _n_! => <br> _a_<sub>1</sub> = 1, _a<sub>n</sub>_ = *n*×*a*<sub>_n_-1</sub> pro _n_ > 1
    - Sčítání posloupností z tělesa _T_ (vektory z *T<sup>n</sup>): (**a**) = (*a<sub>i</sub>*)<sub>*i*≥1</sub> a (**b**) = (*b<sub>i</sub>*)<sub>*i*≥1</sub> => (**c**) = (**a**) ⊕ (**b**) = (*c<sub>i</sub>* = *a<sub>i</sub>* + *b<sub>i</sub>*)<sub>*i\*≥1</sub>
    - Pro číslo α ∈ _T_ α-násobek posloupnosti: (**c**) = α ⊗ (**a**) = (_c<sub>i</sub>_ = α × _a<sub>i</sub>_)<sub>*i*≥1</sub>
    - Množina všech posloupností s takto definovaným sčítáním a násobením tvoří vektorový prostor _S_(_T_) nad tělesem _T_
    - V prostoru nekonečných posloupností lze provádět běžné operace, vytvářet lineární kombinace posloupností, uvažovat o lineárích obalech daných množin a jejich lineární (ne)závislost
    - Je snadné vytvořit nekonečně velkou lineárně nezávislou množinu, ale nepodaří se nám najít množinu v jsjíž lineárním obalu by byly všechny nekonečné posloupnosti - u lineárních kombinací požadujeme **konečný** počet násobků daných vektorů => prostor nekonečných posloupností **ne**má bazi

Zobrazení v posloupnostech

- budou nás nejvíce zajímat zobrazení do jiných vektorových prostorů
- například: _v<sub>M</sub>_ : _S_(_T_) → _T<sup>n</sup>_, které pro danou _n_-tici přirozených čísel _M_ přiřazuje posloupnosti (**a**) _n_-tici hodnot členů posloupnosti _v<sub>M</sub>_(**a**) => lineární zobrazení
- Užitečná jsou i zobrazení nekonečných prostorů do sebe
  - Je-li (**c**) = (_c<sub>i</sub>_)<sub>*i*≥1</sub> ∈ _S_(_T_) pevně daná posloupnost => _n_<sub>(**c**)</sub> : _S_(_T_) → _S_(_T_) definované tak, že _n_<sub>(**c**)</sub>(**a**) = (**d**) = (_c<sub>i</sub>_ · _a<sub>i</sub>_)<sub>*i*≥1</sub> je lineární
- V matematické analýze je významným zobrazením _S_(_T_) → _T_ částečný součet posloupnosti s<sub>n</sub>(**a**) = ∑*a<sub>i</sub>* a zobrazení _s_, které posloupnosti (**a**) přiřazuje posloupnost (**s**) = _s_(**a**) jejích částečných součtů *s<sub>i</sub> = ∑*a<sub>j</sub>\* Obě tato zobrazení jsou také lineární
- posunutí posloupnosti ("zpětné") - (**b**) = _p_(**a**) takž, že *b<sub>i</sub> = *a*<sub>*i\*+1</sub> => lineární zobrazení
- "dopředné" posunutí => není zobrazení, protože nedefinuje prvek _b_<sub>1</sub>, při doplnění hodnoty _b_<sub>1</sub> bychom dostali zobrazení, ale není lineární
  - Lineární zobrazení bychom dostali, kdyby _b_<sub>1</sub> bylo lineární kombinací prvků z (**a**), třeba _b_<sub>1</sub> = 0

Diference

- Δ(**a**) = _p_(**a**) - (**a**) takže [Δ(**a**)]<sub>_i_</sub> = _a_<sub>_i_+1</sub> - _a<sub>i</sub>_ je rozdíl sousedních prvků posloupnosti
- Diference je lineární kombinací lineárních zobrazení, a proto je také lineární
- Protože Δ: _S_(_T_) → _S_(_T_), můžeme vytvářet její mocniny, které se nazývají diferencemi _k_-tého řátu <br> Δ<sup>2</sup>(**a**) = Δ(Δ(**a**))<br>[Δ<sup>2</sup>(**a**)]<sub>_i_</sub> = [Δ(**a**)]<sub>_i_+1</sub> - [Δ(**a**)]<sub>_i_</sub> = _a_<sub>_i_+2</sub> - _a_<sub>_i_+1</sub> - (_a_<sub>_i_+1</sub> - _a_<sub>_i_</sub>) = _a_<sub>_i_+2</sub> -2*a*<sub>_i_+1</sub> + _a_<sub>_i_</sub> <br> a matematickou indukcí lze podle Pascalovy identity dokázat: <br> ![Obecný vzorec](pic/posloupnosti1.png)

Rekurentnost

- O posloupnosti (**a**) řekneme, že je definována rekurentním vztahem *k*tého řádu, pokud _a<sub>n</sub>_ = _f_(_n_,_a_<sub>_n_-1</sub>, _a_<sub>_n_-2</sub>, ..., _a_<sub>_n_-_k_</sub>) pro každé _n_ > _k_
  - Tento rekurentní vztah se nedá použít pro výpočet hodnoty _a<sub>i</sub>_ pro _i_ = 1, 2, ..., _k_. Těchto _k_ počátečních podmínek musíme zadat přímým výčtem
- V systému vztahů<br>![Alt text](pic/posloupnosti2.png)<br>můžeme pomocí diferencí [Δ<sup>*m*</sup>(**a**)]<sub>_n_-_k_</sub> a hodnoty _a_<sub>_n_-_k_</sub> vyjádřit všechny členy _a_<sub>_n_-_k_+1</sub>, _a_<sub>_n_-_k_+2</dub>, ..., _a<sub>n</sub>_ a dosafit za ně do rekurentní definice _k_-tého řádu a dostaneme vztah<br> g* (*n*, *a*<sub>*n*-*k*</sub>, [Δ<sup>1</sup>(**a**)]<sub>*n*-*k*</sub>,...,[Δ<sup>*k*</sup>(**a**)]<sub>*n*-*k*</sub>) = g(*n*, *a*<sub>*n*</sub>, [Δ<sup>1</sup>(**a**)]<sub>*n*</sub>,...,[Δ<sup>*k*</sup>(**a**)]<sub>*n*</sub>) = 0<br>který nazýváme diferenční rovnicí *k\*-tého řádu
- Je-li v rekurentním vztahu *k*tého řádu _a<sub>n</sub>_ = _f_(_n_,_a_<sub>_n_-1</sub>, _a_<sub>_n_-2</sub>,...,_a_<sub>_n_-_k_</sub>) funkce _f_ lineární funkcí parametrů _a<sub>j</sub>_ pro _j_ = _n_-_k_,_n_-_k_+1,...,_n_-1 f*(*n*,*a*<sub>*n*-1</sub>, *a*<sub>*n*-2</sub>,...,*a*<sub>*n*-*k*</sub>) = ∑*c<sub>j</sub>*(*n*)*a*<sub>*n*-*j*+*b*(*n*) kde *b*(n), *c<sub>j</sub>*(*n*) jsou libovolné funkce pořadového čísla *n*, nazýváme vztah *a<sub>n</sub>* = ∑*c<sub>j</sub>*(*n*)*a*<sub>*n*-*j*</sub> + *b*(*n*) lineárním rekurentním vztahem řádu *k\*
  - navíc požadujeme, aby funkce _c<sub>k</sub>_(_n_) nebyla identicky nulová
- definujeme posloupnosti (**b\***), (**c<sub>j</sub>**\*) pro _j_ = 1,2,...,_k_ tak, že _b<sub>i</sub>_\* = _b_(_i_+_k_), (_c<sub>j</sub>_\*)<sub>_i_</sub> = _c<sub>j</sub>_(_i_+_k_) a využijeme podunutí posloupnosti (**a**), můžeme v definici lineárního rekurentního vstahu psát ∑*n*<sub>(**c**<sub>_j_</sub>\*)</sub>(p<sup>_k_-_j_</sup>(**a**)) = -(**b**\*) kde _n_<sub>(**c**<sub>_j_</sub>\*) je zobrazení násobení posloupností (**c**<sub>_j_</sub>\*) a doplněná posloupnost (**c**<sub>0</sub>\*) je konstantní, (_c_<sub>0</sub>\*)<sub>_j_</sub> = -1 pro každé _j_ ∈ _N_
- Klíčovou roli hraje (lineární) zobrazení <br> _L_(**a**) = ∑*n*<sub>(**c**<sub>_j_</sub>\*)</sub>(p<sup>_k_-_j_</sup>(**a**))<br>Formulace úlohy v podobě _L_(**a**) = -**b**\* má tu přednost, že v příznivých případech dovoluje najít explicitní vyjádření členů posloupnosti (**a**).
  - To nazýváme řešením rekurentního vztahu
  - Pro nelineární rekurentní vztahy je taková úloha řešitelná zcela výjimečně
  - Řešení a jeho vlastnosti pro známý vektor (**b**\*) a neznámý vektor (**a**) popisuje Frobeniova věta
  - Odpověď na otázku, jestl je (**b**\*) ∈ _W_(_L_), je kladná a triviálně vyplývá z původní rekurence
- Dalším krokem je nalezení jádra zobrazení _L_ tedy řešení homogenní rovnice _L_(**a**) = (**0**)
- ![Alt text](pic/posloupnosti3.png)

[Kombinatorika ⬅️](./16_Kombinatorika.md) | [➡️ Grafy](./18_Grafy.md)
