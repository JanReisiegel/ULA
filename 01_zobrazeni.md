# Zobrazení

## Definice

- Zobrazení _f_ z množiny _M_ do množiny _N_ je předpis, který každému prvku _m_ ∈ _M_ (vzor) přiřazuje nejvýše jeden prvek _n_ ∈ _N_ (obraz)
- Je-li prvku _m_ ∈ _M_ přiřazen prvek _n_ ∈ _N_, nazýváme _n_ obrazem prvku _m_ při zobrazení _f_
  - _n = f(m)_ - "_n_ je obraz prvku _m_"
- Zápis: _f_: _M_ → _N_ - "zobrazení z množiny _M_ do množiny _N_"
- příklad:
  - _M_ je množina dvojic přirozených čísel a součrt prvků je zobrazení, které dvojici _m_=(_m<sub>1</sub>_,_m<sub>2</sub>_) přiřadí přirozené číslo _f(m)_ = _m<sub>1</sub>_ + _m<sub>2</sub>_
    - pro každý vzor existuje právě jeden obraz
  - _M_ je množina dvojic přirozených čísel doplněných o nulu a podíl se zbytkem je zpobrazení dvojic, které dvojici _m_ = (_m<sub>1</sub>_,_m<sub>2</sub>_) přiřadí dvojici _n_ = (_n<sub>1</sub>_,_n<sub>2</sub>_) takovou, že _m<sub>1</sub>_ = _n<sub>1</sub>_ × _m<sub>2</sub>_ + _n<sub>2</sub>_
    - Pro každý vzor existuje právě jeden obraz s výjimkou -> _m<sub>2</sub>_=0

## Definiční obor

- Ne každému vzoru je při obecném zobrazení přiřazen obraz -> Zavedena množina všech vzorů, kterým lze přiřadit obraz (má smysl obraz hledat)
- Definiční obor zobrazení _f_ je taková podmnožina _D(f)_ množiny _M_, kde pro každé _d_ ∈ _D(f)_ existuje obraz _f(d)_ ∈ _N_
  - Pro prvky množiny _M_, které nejsou v _D(f)_ obraz neexistuje
- **Je-li** _D(f)_ celá množina _M_ => "zobrazení množiny _M_ do množiny _N_"
- **Není-li** _D(f)_ celá množina _M_ => "zobrazení **_z_** množiny _M_ do množiny _N_"

## Obor hodnot

- Obor hodnot zobrazení _f_ je taková podmnožina _W(f)_ množiny _N_, kde pro každé _w_ ∈ _W(f)_ existuje takový prvek _m_ ∈ _M_, že _f(n)_ = _w_
  - Množina všech obrazů, jejichž vzor je neprázdný
- **Je-li** _W(f)_ celá množina _N_ => "zobrazení **na** množinu _N_"
- **Není-li** _W(f)_ celá množina _N_ => "zobrazení **do** množiny _N_

## Vzor prvku oboru hodnot

- Více vzorů se zobrazí do téhož obrazu
- Vzorem prvku _n_ ∈ _N_ je množina _f_ <sup>(-1)</sup>(n)
  - Do této množiny patří všechny prvky z množiny _M_ pro které platí _f(m)_ = _n_
  - Vzor prvku se dá považovat za zobrazení _f_ <sup>(-1)</sup> : _N_ → 2<sup>_M_</sup>
    - 2<sup>_M_</sup> => množina všech podmnožin množiny _M_

## Prosté zobrazení

- Vzorem každého prvku cílové mnnožiny _N_ je nejvýše jednoprvková množina
  - Ke každému obrazu je přiřazen nejvýše jeden vzor
- Zobrazení _f_ : _M_ → _N_ je prosté, pokud pro každé dva prvky _m<sub>1</sub>_ ≠ _m<sub>2</sub>_ z _d(f)_ platí, že _f(m<sub>1</sub>)_ ≠ _f(m<sub>2</sub>)_

## Inverzní zobrazení

- Je-li zobrazení _f_ : _M_ → _N_ prosté, pak zobrazení, které každému _w_ ∈ _W(f)_ přiřazuje prvek _m_ ∈ _M_, kde platí _w_ = _f(m)_, nazveme zobrazením inverzním k _f_
  - Značíme _f_ <sup>-1</sup> a píšeme _m_ = _f_ <sup>-1</sup>(_w_)
- Poté platí:
  - Je-li _f_ : _M_ → _N_, pak _f_ <sup>-1</sup> : _N_ → _M_
  - _D(f_ <sup>-1</sup>_)_ = _W(f)_
  - _W(f_ <sup>-1</sup>_)_ = _D(f)_

## Skládání zobrazení

- Máme-li zobrazení _f_ : _M_ → _N_ a _g_ : _N_ → _O_, pak existuje zobrazení _h_ : _M_ → _O_ složené ze zobrazení _f_ a _g_
  - Platí: _h(m)_ = _g(f(m))_
  - Zapisujeme ve tvaru _h_ = _g(f)_ nebo _h_ = _g_ ◦ _f_

## Identita

- _i<sub>M</sub>_ každému prvku _m_ ∈ _M_ přiřadí znovu tento prvek => identické zobrazení na _M_
  - _i<sub>M</sub>_ : _M_ → _M_
  - _i<sub>M</sub>(m)_ = _m_
- Při skládání zobrazení hraje identické zobrazení roli neutrálního prvku
  - Pro _f_ : _M_ → _N_ je _f_ to samé jako _i<sub>N</sub>(f(i<sub>M</sub>))_
  - Je-li _f_ : _M_ → _N_ prosté zobrazení:
    - _f_ <sup>-1</sup>(_f_) = _i<sub>D(f)</sub>_
    - _f_ (_f_ <sup>-1</sup>) = _i<sub>W(f)</sub>_

[Grafy ⬅️](./18_Grafy.md) | [➡️ Vektorový prostor](./02_VektorovyProstor.md)
