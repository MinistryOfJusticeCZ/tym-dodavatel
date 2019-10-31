# Dokumentace k produktu

## Obecně

* Všechny aplikace Ministerstva spravedlnosti zahrnují telefonní číslo nebo e-mail, kam se uživatelé mohou obrátit ohledně otázek fungování aplikace
* **Před spuštěním aplikací (nebo nových funkcí) musí Tým dodavatele zaslat Dokumentaci k produktu a Video k produktu. Tím zajistí, že bude helpdesk a tým rozvoje připraven odpovídat na otázky týkající se funkčnosti**
* **Tým dodavatele by měl požádat o review Dokumentace k produktu, když**
  1. Kompletní a final build je na staging a Tým si je jist, že je vše připraveno ke spuštění do ostrého provozu
  2. Poté, co dokončil kroky v sekce [Připravte se na review Dokumentace](#pripravte-se-na-review-dokumentace) a
  3. Nejméně 2 týdny před datem spuštění do ostrého provozu
    * Pokud si váš tým myslí, že bude mít potíže s dodržením termínu „2 týdny před spuštěním“, obraťte se na svůj kontakt v Týmu Ministerstva spravedlnosti

## Připravte se na review Dokumentace

### Krok 1: Vytvořte Dokumentaci k produktu

*Pokud budujete zcela novou službu*:

  1. Vytvořte Dokumentaci k produktu, která bude pokrývat všechny funkcionality, primární user flow(s), jakékoli chybné stavy a jak může uživatel tyto chyby vyřešit
  2. Dokumentace k produktu musí být buď Word dokument nebo PDF
  3. Vytvořte novou složku v Gitu pod vaším projektem s názvem ```Dokumentace```. Do ní vložte Dokumentaci k produktu

*Pokud budujete nové funkce pro již existující službu*:

  1. Je potřeba aktualizovat existující Dokumentaci k produktu
      * Pokud nemůžete existující Dokumentaci k produktu na Gitu nalézt, kontaktujte Tým Ministerstva spravedlnosti
  2. Vložte aktualizovanou Dokumentaci k produktu na původním místě

*Příklady*:

TODO

### Krok 2: Vytvořte Video k produktu 

*Pro nové služby a aktualizace do stávajících*:

1. Vytvořte a Video k produktu (se zvukem), které ukazuje primární user flows
2. Abyste si byli jisti, že jste pokryli vše, zkontrolujte Video k produktu s věcným garantem
3. Vytvořte slovní přepis z audia k Videu k produktu. Slovní přepis musí být Word dokument nebo PDF
4. Pokračujte k [Požadavku na review Dokumentace](#pozadavek-na-review-dokumentace)

## Požadavek na review Dokumentace

1. Vytvořte issue do ```složky [NÁZEV_PROJEKTU]/[NÁZEV_PROJEKTU]-tym-dodavatel``` na Gitu
    * Název/Title: ```Požadavek na review Dokumentace```
    * Štítky/Labels:
      * ```helpdesk```
      * ```externi-pozadavek```
      * ```[label vašeho týmu]```, např. „DUHA“
    * Přiřaďte problém/Assignee: ```hlavsa```
    * Komentář: Uveďte následující informace
      * **Kontext**: Poskytněte kontext projektu
        * např. ```Funkčnost přidává nový dataset, takže uživatelé mohou vyhledávat a prohlížet svůj stav na mapě.```
      * **URL**: ```odkaz na projekt na stagingu```
      * **Dokumentace k produktu**: ```odkaz na Dokumentaci k produktu na Git```
      * **Video k produktu**: ```odkaz na Video k produktu```
      * **Video k produktu přepis**: ```odkaz na slovní přepis Videa k produktu```      

2. **Během 3 pracovních dní** Tým Ministerstva odešle Dokumentaci k produktu, Video k produktu, a slovní přepis Videa k produktu helpdesku a týmu rozvoje
    * Pokud se do 3 pracovních dnů nic nestane, obraťte se na svůj kontakt na Ministerstvu
3. Po odeslání všech materiálů, problém uzavřete
4. Po uzavření issue přijde tvůrci issue notifikace, tím se tato aktivita považuje za dokončenou
