# Best practices pro přístupnost

**Obsah na této stránce**

- [Best practices pro přístupnost](#best-practices-pro-pristupnost)
  - [Sémantický markup](#semanticky-markup)
  - [Design System](#design-system)
  - [Automatizované testování přístupnosti](#automatizovane-testovani-pristupnosti)
  - [Manuální testování přístupnosti](#manualni-testovani-pristupnosti)
    - [Zoom na 400 %](#zoom-na-400)
    - [Navigace pomocí klávesnice](#navigovani-pomoci-klavesnice)
    - [Odečítačky obrazovek](#odecitacky-obrazovek)
    - [Testy barev](#testy-barev)
  - [Pokračovat ve čtení](#pokracovat-ve-cteni)

## Sémantický markup

- Periodicky kontrolujte vyrenderované HTML, zvlášť během vývoje. Ujistěte se, že je HMTL validní proti `HTML5` doctype
- Každá stránka by měla mít jako první nadpis (heading) H1
- Nadpisy jdou správně postupně za sebou:
  - H1 vyjadřuje účel stránky
  - H2 jsou používány k sémantické definici vysoko-úrovňových skupin s obsahem (nadpis odstavce, nadpis podstránky)
  - H3 až H5 by měl být používán k definování podčástí
  - H6 se nepoužívá
- `<title>` tagy stránky jsou aktualizovány každou změnou URL
  - Text H1 je obsažen v názvu stránky
  - Název stránky může být delěí nebo více popisný než H1
  - Například, `<h1>` může říct "Zjistěte více o výhodách" a `<title>` může říct "Zjistěte více o výhodách | Justice.cz"

## Design System

- Použijte [Frontend](https://github.com/MinistryOfJusticeCZ/frontend) jako základ pro vizuální design
- Více na [GOV.UK Design System](https://design-system.service.gov.uk)

## Automatizované testování přístupnosti

1. Front-end vývojáři by měli být nainstalovány [aXe plugin pro Chrome nebo Firefox](https://deque.com/axe) a pravidelně jej spouštět během své práce
2. Build server spustí aXe sken na všech vyrenderovaných stránek v Kroku 2. aXe skeny zkontrolují, zda stránka splňuje Section 508, WCAG2 A a WCAG2 AA
3. **Každá vyrenderovaná stránka musí projít aXe kontrolou**
    * Statické Markdown stránky musí být zkontrolovány aXe plugin
    * Stránky vytvořené pomocí content management system (CMS) musí být zkontrolovány aXe pluginem

## Manuální testování přístupnosti

### Zoom na 400 %

- Nastavte šířku prohlížeče na 1280px
- Přibližte stránky stisknutím `Ctrl a +` na Windows nebo `Cmd a +` na Mac, pokud přohlížeš nepřiblíží stránku na 400 %.
- Většina obsahu nesmí scrollovat do stran. Horizontální scrollování je povoleno pouze pro obsah jako obrázky, mapy, diagramy, prezentace, a datové tabulky
- [Understanding Success Criterion 1.4.10: Reflow](https://www.w3.org/WAI/WCAG21/Understanding/reflow.html)
- [WCAG: Understanding Reflow](https://www.w3.org/WAI/WCAG21/Understanding/reflow.html)

### Navigace pomocí klávesnice

- Ujistěte se, že všechny prvky, které přijímají stav :focus (odkazy, vstupní pole formuláře, tlačítka, přepínače, zaškrtávací pole) jsou dosažitelné klávesnicí. Ujistěte se, že jakékoliv prvky s `tabIndex="0"` jsou normálně fokusovatelné
- Tam, kde je to možné, používejte vhodné sémantické prvky
- Vyhněte se pastím na klávesy. Jedná se o situace, kdy se uživatelé mohou pomocí klávesy `TAB` někam v interfacu dostat, ale dalším stiskem klávesy `TAB` nebo `SHIFT+TAB` se z něj už nedostanou
- Ujistěte se, že vaše aplikace má předvídatelné pořadí prvků (tabbing order). V jazycích, kde se čte zleva-doprava, shora dolů. V několika sloupcových pohledech použijte svůj nejlepší úsudek. Interfacy, které obsahují levé navigační menu, zpravidla umožňují fokus pro každý odkaz nebo tlačítko v levém menu, a pak přesunout fokus do místa s hlavním obsahem
- Nabídněte možnosti, jak přeskočit velkou část textu, jako je [odkaz na přeskočení obsahu](https://webaim.org/techniques/skipnav/)
- Oveřte fungování pomocí [WebAIM návodu jaké se používají klávesy](https://webaim.org/techniques/keyboard/)

### Odečítačky obrazovek

-  Průchod stránkou musí být možný na [Ministerstvem spravedlnosti podporovaných prohlížích](/pristupnost/podporovane-prohlizeče.md) s nejčastěji používanými odečítačkami (například [2017 WebAIM dotazník ohledně odečítaček](https://webaim.org/projects/screenreadersurvey7/)):

  - [ ] Uživatel musí stránkou procházet pouze za pomoci klávesnice (bez žádného ukazovacího zařízení). Podívejte se na [WebAIM návod jaké se používají klávesy](https://webaim.org/techniques/keyboard/)
  - [ ] Windows 7/10: IE11 s JAWS
  - [ ] Windows 7/10: Chrome s JAWS
  - [ ] Windows 7/10: Firefox s NVDA
  - [ ] MacOS: Safari s Voice Over. Ujistěte se, že máte před testováním [zapnuté funkce Zpřístupnění](https://www.scottohara.me/blog/2014/10/03/link-tabbing-firefox-osx.html).

### Testy barev

Testujte barvoslepost pomocí nástrojů jako:
- [Chrome Colorblinding plugin](https://chrome.google.com/webstore/detail/colorblinding/dgbgleaofjainknadoffbjkclicbbgaa?hl=en)
- Sketch plugin, [Color Contrast Analyser](https://github.com/getflourish/Sketch-Color-Contrast-Analyser)
- [Barevná paleta GOV.UK Design System](https://design-system.service.gov.uk/styles/colour/)

## Pokračovat ve čtení
Zkratkovitě tomůžete přístupnost pochopit pomocí plakátů na url: https://github.com/MinistryOfJusticeCZ/plakaty/tree/master/accessibility/dos-donts/posters_cz
