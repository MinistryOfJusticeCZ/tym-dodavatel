# Určování závažnosti defektů přístupnosti
Tento dokument bude poskytovat společný jazyk pro určování závažnosti defektů týkajích se přístupnosti. Zachycuje následující:

1. Závažnost defektu
2. Dopad na potenciální uživatele ovlivněné defektem
3. Časový rámec, ve kterém by měla být vada odstraněna

## pristupnost-defekt-0 (Showstopper)

### Typ problému:
* Past na klávesy (2.1.2 WCAG)
* Obsah není dosažitelný bez ukazovacího zařízení jako je myš (custom nebo nativní elementy)
* [Rychlé záblesky](https://www.w3.org/TR/UNDERSTANDING-WCAG20/seizure-does-not-violate.html) (může spustit epileptický záchvat)
* Pohyby nebo hýbající se obsah, který zakrývá velké procento obrazovky (možné [vestibulární problémy](https://a11yproject.com/posts/understanding-vestibular-disorders/))

### Dopad na potenciální uživatele
* Navigace pomocí klávesnice
* Odečítačka obrazovky nebo jiná asistenční pomůcka
* Uživatele, kteří mají poruchy zraku nebo jsou slepí
* Uživatele, kteří mají problémy se sluchem nebo jsou hlušší
* Ti, kdo mají [vestibulární problémy](https://a11yproject.com/posts/understanding-vestibular-disorders/) jako pohybová nevolnost
* Ti, kdo jsou fotosenzitivní

### Doba pro fix
* Problém musí být spraven před spuštěním

## pristupnost-defekt-1 (Kritický)

### Typ problému:
* Kritické chyby (critical errors) v automatizovaných testerech jako jsou [aXe plugin](https://www.deque.com/axe), [SortSite](https://www.powermapper.com/products/sortsite/), [AATT](https://github.com/paypal/AATT)
* Nepřístupný obsah bohatý na informace jako video je bez titulků
* Problémy s barevným kontrastem
* Chybějící názvy formulářových polí
* Dynamický obsah je přidáván nebo odstaraňován ze stránky bez ohlášení změny asistenčním pomůckám
* UI nebo prvnky formuláře nejsou dosažitelné klávesou `TAB` nebo `SHIFT + TAB`
* Obsah bez jasného označení stavu :focus

### Dopad na potenciální uživatele
* Navigace pomocí klávesnice
* Odečítačka obrazovky nebo jiná asistenční pomůcka
* Uživatele, kteří mají poruchy zraku nebo jsou slepí
* Uživatele, kteří mají problémy se sluchem nebo jsou hlušší

### Doba pro fix
* Problém je prioritozován a je spraven, pokud možno, v dalším sprintu

## pristupnost-defekt-2 (Vážný)

### Typ problému:
* Vážné chyby (serious errors) v automatizovaných testerech jako jsou [aXe plugin](https://www.deque.com/axe), [SortSite](https://www.powermapper.com/products/sortsite/), [AATT](https://github.com/paypal/AATT)
* Přiblížený text je použitelný pouze za pomoci horizontální scrollování, text těžko k přečtení
* Problémy pro barvoslepé (například, barva je jediným nositelem informace)
* Názvy polí nebo tlačítka nejsou dostatečně popisná pro asistenční pomůcky ("Editovat...co?")
* Dynamický obsah je přidáván nebo odstaraňován ze stránky bez ohlášení změny asistenčním pomůckám
* Obsah, který nedává smysl mimo kontext, nebo neobsahuje vůbec žádné vysvětlení
* Chybějící landmarky HTML. To znamená, banner, navigation, main, aside, footer prvky, nebo divy s role atributy.
* Nevhodné nadpisy, zanořování
* Nevhodné ARIA atributy, chybějící ID
* [Neřízení fokusu v single-page aplikacích](https://adhocteam.us/2018/02/20/developer-driven-focus-management-for-single-page-applications/)

### Dopad na potenciální uživatele
* Navigace pomocí klávesnice
* Odečítačka obrazovky nebo jiná asistenční pomůcka
* Uživatele, kteří mají poruchy zraku nebo jsou slepí
* Uživatele, kteří mají problémy se sluchem nebo jsou hlušší
* Uživatele mající problémy s krátkodobou pamětí nebo jinými kognitivními problémy

### Doba pro fix
* Problém je prioritozován a je spraven, pokud možno, mezi 1 až 3 sprintem

## pristupnost-defekt-3 (Méně významný)

### Typ problému:
* Méně významné chyby (minor errors) v automatizovaných testerech jako jsou [aXe plugin](https://www.deque.com/axe), [SortSite](https://www.powermapper.com/products/sortsite/), [AATT](https://github.com/paypal/AATT)
* Invalidní HTML (nesémantické, špatně strukturované)

### Dopad na potenciální uživatele
* Navigace pomocí klávesnice
* Odečítačka obrazovky nebo jiná asistenční pomůcka
* Uživatelé se slabozrakostí

### Doba pro fix
* Problém je měl být prioritizován pro nadcházející iteraci (často dlouhou 3 sprinty)
* Tyto problémy jsou často věci, které vývojáři opravují, pokud mají několik hodin navíc před koncem sprintu

## pristupnost-defekt-4 (Triviální)

### Typ problému:
* Triviální chyby (trivial errors) v automatizovaných testerech jako jsou [aXe plugin](https://www.deque.com/axe), [SortSite](https://www.powermapper.com/products/sortsite/), [AATT](https://github.com/paypal/AATT)
* Invalidní HTML (nesémantické, špatně strukturované)
* Méně sémantické HTML (například, používání `<ul>` namísto `<ol>` pro sekvenční instrukce)

### Dopad na potenciální uživatele
* Navigace pomocí klávesnice
* Odečítačka obrazovky nebo jiná asistenční pomůcka
* Uživatele, kteří mají poruchy zraku nebo jsou slepí
* Uživatele mající problémy s krátkodobou pamětí nebo jinými kognitivními problémy

### Doba pro fix
* Problém je měl být prioritizován pro nadcházející iteraci (často dlouhou 3 sprinty)
* Tyto problémy jsou často věci, které vývojáři opravují, pokud mají několik hodin navíc před koncem sprintu
