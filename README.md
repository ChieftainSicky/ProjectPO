# ProjectPO

## Scénář
Vývojový scénář k aplikaci generující SQL script pro databázové specialisty.  
Účelem programu je načíst data získána ze vstupních souborů, které reprezentují určitý stav databáze. A na základě těchto vstupních dat provádět specifické operace. Například generování scriptu pro vytvoření nové DB nebo upgrade té stávající. Tyto operace následně vygenerují SQL script, který lze spustit.  

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
* Návrh fungování aplikace -> 4h (1h)
* Návrh gui (návaznost, jednoduchost, přehlednost) -> 3h (1h)
* Návrh podoby výstupních souborů (sql script) -> 3h (1h)

### Vývoj
* Programování - parseru vstupních datových modelů -> 4h (8h)
* Programování - metod volaných z gui a jejich návaznost na modely -> 3h (5h)
* Programování - metod, které generují výsledný skript -> 4h (16h)
* Programování - custom messengeru, vypisujícího hlášky do WPF -> 2h (3h)
* Programování - instalátoru -> 2h (8h)

### Testování
* Testování parseru -> 2h (2h)
* Testování generování skriptu -> 2h (4h)
* Testování správnosti ostatních metod a messengeru -> 3h (2h)
* Sepsání dokumentace -> 3h (2h)

## Otázky
* Lze zrychlit? (Načítání, generování, výpis, ukládání, GUI)
* Lze modifikovat? (schopnost adaptace novým změnám, požadavkům)

# Reálně

## Časový plán
100% ~ 53h  
&ensp; 5,7% -> analýza (3h)  
&ensp; 75,5% -> vývoj (20h)  
&ensp; 18,8% -> testování, ladění (10h)

### Analýza
* Návrh fungování aplikace ~ 1h
* Návrh gui (návaznost, jednoduchost, přehlednost) ~ 1h
* Návrh podoby výstupních souborů (sql script) ~ 1h

### Vývoj
* Programování - parseru vstupních datových modelů ~ 8h
* Programování - metod volaných z gui a jejich návaznost na modely ~ 5h
* Programování - metod, které generují výsledný skript ~ 16h
* Programování - custom messengeru, vypisujícího hlášky do WPF ~ 3h
* Programování - instalátoru ~ 8h

### Testování
* Testování parseru ~ 2h
* Testování generování skriptu ~ 4h
* Testování správnosti ostatních metod a messengeru ~ 2h
* Sepsání dokumentace ~ 2h
