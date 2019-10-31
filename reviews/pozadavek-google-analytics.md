# Požadavek na zavedení Google Analytics - NÁVRH NEPOUŽÍVAT

### Pozor

* **Všechny týmy pracující na službách pro Ministerstvo spravedlnosti musí integrovat Google Analytics do svých služeb**
* **Tým dodavatele by měly o Google Analytics požádat, když:**
  * Kompletní a final build je na staging a je si jist, že je připraven ke spuštění.
  * Nejméně 4 týdny před plánovaným datem zahájení:
    - nutná koordinace s týmem Ministerstvem spravedlnosti
    - potřeba validace na stagingu

### Připravte se na Google Analytics

Odpovězte na následující otázky v dokumentu Word:

* Jaké kroky byste chtěli měřit, abyste pochopili progres a odchod (abandoment)?
* Jaké další interakce uživatelů, kromě například Tisk nebo Uložit, jsou klíčem k pochopení chování uživatelů?
* Jaké další prvky navigace na webu vám pomohou pochopit, jak uživatelé navigují a používají vaši službu?
* Jaké metriky úspěchu jste pro službu identifikovali?
* Jakou uživatelskou interakci nebo chování chcete počítat jako „transakci“, kterou chcete sledovat? Jaké jsou vaše cíle pro každou z těchto transakcí?
* Jaké vlastní dimenze (pokud existují) byste chtěli sbírat? Mohou to být uživatel, relace (session) nebo produkt.
* Jaké další události (events), interakce, chování (behavior), které nejsou pokryty výše uvedenými otázkami, chcete sledovat?

### Požadavek na Google Analytics

1. Vytvořte issue do ```složky [NÁZEV_PROJEKTU]/[NÁZEV_PROJEKTU]-tym-dodavatel``` na Gitu
    * Název/Title: ```Požadavek na Google Analytics```
    * Štítky/Labels:
      * ```analytics```
      * ```externi-pozadavek```
      * ```[label vašeho týmu]```, např. „DUHA“
    * Přiřaďte problém/Assignee: ```hlavsa```
    * Popis/Description: Uveďte následující informace:
      * **Kontext:** Poskytněte kontext projektu
        * např. ```Funkčnost přidává nový dataset, takže uživatelé mohou vyhledávat a prohlížet svůj stav na mapě.```
        * **URL:** ```odkaz na váš projekt na staging```
      * **Přílohy:** ```Nahrajte Word dokument, který jste vyplnili podle otázek výše```
2. **Do 4 pracovních dnů** Tým Ministerstva spravedlnosti předá požadavek příslušnému členu týmu, aby vám zajistil přístup
    * Pokud se do 4 pracovních dnů nic nestane, obraťte se na svůj kontakt na Ministerstvu
    * Ve chvíli, kdy Tým Ministerstva spravedlnosti shromažďuje informace potřebné k nastavení GA, je možné, že mohou v komentářích k tomuto issue být vyžádány další podklady
3. Ve chvíli, kdy je toto vyřízeno, Tým Ministerstva aktualizuje issue
    * *Pokud jsou vyžadovány custom události (events), Ministerstvo:*
      1. Aktualizuje issue s popisem, jak custom events implementovat do kódu
      1. Tým dodavatele provede nutné změny v kódu a pushne je na staging
      1. Tým dodavatele aktualizuje issue s komentářem: ```Custom events jsou nastaveny```
    * *Pokud nejsou vyžadovány custom události (events)*, Ministerstvo přejde na další krok
4. Tým Ministerstva spravedlnosti ověří, že Google Analytics fungují na stagingu
    * Během verifikace, Tým Ministerstva spravedlnosti může najít problémy, které povedou ke změně kódu nebo něco, co je třeba změnit přes Google Tag Manager. Pokud se tak stane, Tým Ministerstva spravedlnosti aktualizuje issue s instrukcemi, jak to udělat
      * Jakmile Tým dodavatele spraví tyto problémy, aktualizuje issue a požádá Tým Ministerstva o znovu-ověření
5. Ve chvíli, kdy je Tým Ministerstva spravedlnosti přesvědčený, že Google Analytics fungují správně, provede:
    * Přidání komentáře v issue: ```GA připraveno```
    * Zavře issue.
6. Po ukončení problému se tato aktivita před spuštěním považuje za dokončenou


### Používání Google Analytics

Pokud váš tým bude i **po spuštění** neustále vylepšovat (nebo udržovat) službu, musí být vytvořen účet na Google Analytics.

* Každé osobě, která bude používat Google Analytics, je potřeba vytvořit nový účet Google Analytics

Pokud chcete tyto účty vytvořit:

1. Vytvořte issue do ```složky [NÁZEV_PROJEKTU]/[NÁZEV_PROJEKTU]-tym-dodavatel``` na Gitu
    * Název/Title: ```Provision Google Analytics```
    * Štítky/Labels:
      * ```analytics```
      * ```externi-pozadavek```
      * ```[label vašeho týmu]```, např. „DUHA“
    * Přiřaďte problém/Assignee: ```hlavsa```
    * Popis/Description: Uveďte následující informace:
      * **Kontext:** Poskytněte kontext projektu
        * např. ```Seznam účtů na Google Analytics společně s jmény osob a jejich e-mailových adres.```
2. **Do 4 pracovních dnů** Tým Ministerstva spravedlnosti zřídí tyto účtu, abyste mohli začít používat Google Analytics
    * Pokud se do 4 pracovních dnů nic nestane, obraťte se na svůj kontakt na Ministerstvu
3. Ve chvíli, kdy Ministerstvo tyto účty zřídí, tak
    * Přidá komentář k issue: ```Google Analytics účty zřízeny```
    * Zavře issue
4. Po uzavření issue přijde tvůrci issue notifikace. To je signál pro váš tým začít používat Google Analytics
5. Jakékoli další změny ohledně implementace GA řešte skrz issues