# Cvičení: Společné účty – menu, zobrazení a filtrování dat ze souboru

## Téma
Skupina kamarádů si na výletě zapisuje výdaje. Na konci výletu si chtějí spočítat, kolik kdo musí přispět do společné pokladny, ze které výdaje platí. 

## Zadání:

Vytvořte aplikaci s&nbsp;grafickým uživatelským rozhraním, která bude splňovat následující požadavky:
- Aplikace bude mít dvě (jednořádková) textová pole. Jedno pro zadání filtru názvu (jména kamaráda) a druhé pro zobrazení výsledku (celkového dluhu do společné pokladny). Dále bude v UI tlačítko „Filtruj“.
- Pole pro zobrazení výsledku není možné editovat – pouze zobrazuje výsledek. (Pole pro zadání jména kamaráda editovat lze.)
- Aplikace bude číst data z textového souboru ve formátu:
    > Jméno kamaráda : částka  

    Příklad vstupního souboru: 
    > Eva : 350  
    > Adam:   500  
    > Alex :180  
    > Eva : 35  
    > Adam : 100

    Počítejte s tím, že kolem dvojtečky někdy jsou mezery a jindy nejsou – soubor byl generován ručně. Mezer tam může být více, nejsou tam ale žádné jiné znaky kromě mezer.

    Jména v souboru se můžou opakovat, protože jeden kamarád nakupuje více položek.

- Přidejte do menu aplikace položky:
    - _Soubor > Načti..._ zobrazí dialog pro výběr souboru a načte data ze souboru do vhodně strukturovaného seznamu
    - _Soubor > Ulož výsledky..._ zobrazí dialog pro výběr souboru a uloží data do výstupního souboru ve tvaru:
        > Jméno kamaráda => celková částka

        Například:
        > Eva => 385  
        > Adam => 600  
        > Alex => 180

        Každé jméno je ve výstupním souboru jen jednou a za ním je uvedena celková sečtená částka všech položek daného kamaráda.
    - _Akce > Zobraz statistiku_... Tato akce zobrazí vyskakovací okno, kde budou uvedena jména všech kamarádů a u každého celkovou částku všech jeho nákupů.
    - _Nápověda_... Zobrazí vyskakovací okno s textem „Zadej jméno s stiskni tlačítko Filtruj!“

- Obsah pole pro zobrazení výsledku: 
    - Ve výstupním poli se bude zobrazovat nula, pokud není načtený žádný soubor.
    - Pokud načteme soubor a pole se jménem kamaráda je prázdné, zobrazí se ve výstupním poli celková cena všech nákupů.
    - Pokud je soubor načten a v poli se jménem kamaráda je vyplněné jméno, zobrazí se ve výstupním poli celková cena nákupů daného kamaráda (nula, pokud se jméno v seznamu nevyskytuje).
    - Po zadání jména kamaráda je třeba stisknout tlačítko „Filtruj“, aplikace nemusí reagovat na změnu ve vstupním poli bez stisknutí tlačítka.

- Vhodně ošetřete chyby při práci se soubory a chybu zobrazte ve vyskakovacím okně.

## Vzhled aplikace
![](00200-soubor-menu.png)

