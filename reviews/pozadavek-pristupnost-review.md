# Požadavek na pre-launch review přístupnosti

**Obsah stránky**

- [Splnění přístupnosti a zákona 99/2019](#splneni-pristupnosti-a-zakona-99/2019)
- [Krok 1: Pročtěte si dokument s Best practices pro přístupnost](#krok-1-proctete-si-dokument-s-best-practices-pro-pristupnost)
- [Krok 2: Požadavek na review přístupnosti](#krok-2-pozadavek-na-review-pristupnosti)
- [Krok 3: Review Ministerstva](#krok-3-review-ministerstva)

## Splnění přístupnosti a zákona 99/2019

**Všechny aplikace a služby, které běží na Ministerstvu spravedlnosti musí být přístupné a splňovat zákon 99/2019.** Zjednodušeně to znamená splnit kritéria úrovně A a AA standard [Web Content Accessibility Guidelines (WCAG)](https://www.w3.org/TR/WCAG20/).

## Krok 1: Pročtěte si dokument s Best practices pro přístupnost

1. Pročtěte si nejnovější [best practices pro přístupnost](pristupnost/pristupnost-best-practices.md) Ministerstva spravedlnosti
2. Vytvořte issue pro jakýkoliv bod, který byste s Týmem Ministerstva rádi prodiskutovali

## Krok 2: Požadavek na review přístupnosti

1. Vytvořte [požadavek na review přístupnosti před spuštěním služby](https://github.com/MinistryOfJusticeCZ/tym-dodavatel/issues/new?labels=př%C3%ADstupnost%2C+review%2C+extern%C3%AD+tým&template=pristupnost-review-sablona.md&title=Požadavek+na+review+př%C3%ADstupnosti+pro+NÁZEV_PRODUKTU)
2. **Během 5 pracovních dnů**, Tým Ministerstva zkontroluje váš kód a dá vám vědět výsledky
   - Pokud se do 5 pracovních dnů nic nestane, obraťte se na svůj kontakt na Ministerstvu
3. _Jsou-li nalezeny problémy_, Tým Ministerstva vytvoří nové issue pro každý nalezený problém s přístupností
   - Issues budou přiděleny osobě, která je vytvořila v kroku 3
   1. Každé issue popisuje konkrétní změny potřebné k tomu, aby byl kód přístupný - co je problém, kde se problém vyskytuje, jak jej opravit a závažnost problému
   2. **Očekává se, že váš tým provede všechny změny před spuštěním** Ve chvíli, kdy Tým dodavatele změny dokončí, aktualizuje každé issue následujícím komentářem
      - `Změny v tomto kódu jsou dokončené [odkaz na staging]`
   3. Zavřete všechny issues
   4. Po zavření všech issues se tato aktivita považuje za dokončenou
   5. Tým Ministerstva poté dělá [Krok 3](#krok-3-review-ministerstva).
4. _Nejsou-li nalezeny žádné problémy_,
   1. Tým Ministerstva aktualizuje původní issue tímto komentářem: „Nebyly nalezeny žádné problémy“
   2. Tým Ministerstva issue uzavře
   3. Git pošle tvůrci issue oznámení. To je signál pro Tým dodavatele, že je tato aktivita dokončena.
   - Tým Ministerstva poté dělá [Krok 3](#krok-3-review-ministerstva)

## Krok 3: Review Ministerstva

Protože veškerý kód na Ministerstvu spravedlnosti prochází přísným manuálním a automatickým testováním:

1. Jednou za měsíc Ministerstvo spravedlnosti prochází veškerý kód předložený v předchozích 30 dnech

2. Zkontroluje kód a poskytne zpětnou vazbu / pokyny Týmu dodavatele

3. Ministerstvo spravedlnosti může požadovat další změny vašeho kódu. Pokud k tomu dojde, Tým Ministerstva vytvoří nové issue pro každý problém s přístupností.
   - Issues budou přiděleny osobě, která je vytvořeny v [počátečním přezkumu v Kroku 2](#krok-2-pozadavek-na-review-pristupnosti).
   - Každý problém popisuje konkrétní změny potřebné k zajištění souladu se zákonem 99/2019 - jaký je problém, kde se problém vyskytuje, jak jej opravit a závažnost problému.

4. **Očekává se, že váš tým provede všechny změny co nejrychleji, například v příštím sprintu po obdržení požadovaných změn.**
   - Po dokončení změn aktualizujte každé issue následujícím komentářem?
     - `Změny v tomto kódu jsou dokončené [odkaz na staging]`
   - **NEZAVÍREJTE** issue
   - Tým Ministerstva spravedlnosti potvrdí změny a zavře issue
