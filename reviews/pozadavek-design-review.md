# Požadavek na pre-launch review UX/IxD/UI a vizuální designu

### Pozor

* **Všechny týmy pracující na službách pro Ministerstvo spravedlnosti jsou povinni dodržovat pokyny a patterny [Frontendu Ministerstva spravedlnosti](https://github.com/MinistryOfJusticeCZ/frontend).**
* **Tým dodavatel by měl naplánovat Design QA, kdy je final build na staging.**
  * Design QA by mělo nastat, když je tým přesvědčen, že před spuštěním nedojde k žádným dalším změnám.

## Požádejte o Design QA

1. Vytvořte issue do ```složky [NÁZEV_PROJEKTU]/[NÁZEV_PROJEKTU]-tym-dodavatel``` na Gitu
    * Název/Title: ```Požadavek na Design QA```
    * Štítky/Labels:
      * ```design```
      * ```externi-pozadavek```
      * ```[label vašeho týmu]```, např. „DUHA“
    * Přiřaďte problém/Assignee: ```hlavsa```
    * Popis/Description: Uveďte následující informace:
      * **Kontext:** Poskytněte kontext projektu
        * např. ```Funkčnost přidává nový dataset, takže uživatelé mohou vyhledávat a prohlížet svůj stav na mapě.```
      * **URL:** ```odkaz na váš projekt na staging```
      * **Nové design patterny (pokud existují):** Poznamenejte místa, kde jste vytvořili a použili nové design patterny (pokud existují)
      * **Design challenges (pokud existují):** Poznamenejte neobvyklé nebo složité problémy s designem, které jste v této práci potřebovali vyřešit.
      * TODO - zde příklad
2. **Do 4 pracovních dnů** Tým Ministerstva spravedlnosti provede Design QA pomocí [Kontrolního seznamu níže](#design-qa-checklist)
    * Pokud se do 4 pracovních dnů nic nestane, obraťte se na svůj kontakt na Ministerstvu
3. Tým ministerstva spravedlnosti aktualizuje issue pomocí snímků obrazovky a ukáže vám, kde je třeba změnit design
4. Dokončete všechny požadované změny na přiložených snímcích obrazovky
    * Pokud má váš tým dotazy (nebo nesouhlasí s požadovanou změnou), použijte issue na Gitu
5. Po vypořádání všech změn, problém uzavřete
6. Po uzavření issue přijde tvůrci issue notifikace, tím se tato aktivita považuje za dokončenou

## Otázky pro osobní review designu

1. Co je tou potřebou uživatele?
2. Je to, co to říká, a to co to dělá skutečně to samé?
3. Co si jako uživatel odnesu po 3 sekundách? (Pravidlo je 8 sekund.)
4. Kdo to potřebuje vědět?
5. Co někdo co předtím nevěděl, ví teď?
6. Proč to stojí kliknutí?
7. Nepředpokládáme až moc?
8. Proč takové pořadí?
9. Co se stane, když se zbavíme tohohle?
10. Jak to můžeme udělat více očividné/jasné?

## Design QA Checklist

* [ ] Tým Ministerstva spravedlnosti nové design patterny zkontroloval a zdokumentoval
* [ ] Byly zohledněny breakpointy pro mobily, tablety a počítače
* [ ] Správné použití design patternů v kontextu
* [ ] Správné použití typografie
* [ ] Padding a spacing byly použity správně
* [ ] Komponenty formuláře byly v kontextu použity správně
* [ ] Konzistentní používání ikonografie
* [ ] Použití barev je v souladu s paletou barev
* [ ] Primární a sekundární tlačítka správně použita v kontextu
* [ ] :hover a :focus stav byly zohledněny a jsou v souladu s design patterny
* [ ] Výstražné zprávy byly použity odpovídajícím způsobem
* [ ] Chybové stavy byly zohledněny a použity odpovídajícím způsobem
* [ ] V případě potřeby byly použity ukazatele načítání (loading indicator)
