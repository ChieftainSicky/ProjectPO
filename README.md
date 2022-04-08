# ProjectPO

## Scénář
Vývojový scénář k aplikaci generující SQL script pro databázové specialisty.  
Účelem programu je načíst data získána ze vstupních souborů, které reprezentují určitý stav databáze. A na základě těchto vstupních dat provádět specifické operace. Například generování nové DB nebo upgrade stávající. Tyto operace následně vygenerují SQL script, který lze spustit.  

## Požadavky
* Jednoduchost
* Rychlost
* Robustnost
* Rozšiřitelnost

## Technologie 
* vývojové prostředí - C#
* fasáda aplikace - WPF
* distribuce - .msi instalátor

## Časový plán
100% = 40h  
&ensp; 25% -> analýza (10h)  
&ensp; 50% -> vývoj (20h)  
&ensp; 25% -> testování, ladění (10h)

## Požadavky v bodech 

### Analýza
* Návrh fungování aplikace -> 4h
* Návrh gui (návaznost, jednoduchost, přehlednost) -> 3h
* Návrh podoby výstupních souborů (sql script) -> 3h

### Vývoj
* Programování - parseru vstupních datových modelů -> 4h
* Programování - metod volaných z gui a jejich návaznost na modely -> 3h
* Programování - metod, které generují výsledný skript -> 4h
* Programování - custom messengeru, vypisujícího hlášky do WPF -> 2h
* Programování - instalátoru -> 2h

### Testování
* Testování parseru -> 2h
* Testování generování skriptu -> 2h
* Testování správnosti ostatních metod a messengeru -> 3h
* Sepsání dokumentace -> 3h

## Otázky
* Lze zrychlit? (Načítání, generování, výpis, ukládání, GUI)
* Lze modifikovat? (schopnost adaptace novým změnám, požadavkům)
