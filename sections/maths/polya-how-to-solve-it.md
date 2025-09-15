---
layout: default
title: "Polya: How to Solve it"
section_order: 9
section_key: maths
date: 2025-09-13
permalink: /mathematics/polya-how-to-solve-it
---

# Four methods

Jelikož brzy budu vést cvičení z diskrétní matematiky na MFF UK. Začal jsem si číst tuto pěknou knížku od George Polyi. Měla by člověka naučit, jak efektivně řešit matematické problémy. Myslím si, že je to dovednost, která je dobrá umět i do běžného života. Spoustu strategií, které člověk při řešení matematických problémů používá se dá využít i při řešení problémů všedních.

Polya představuje tuto obecnou čtyřbodovou strategii, jak problémy řešit:
1. Understanding the problem
2. Devising a plan
3. Carrying out the plan
4. Looking back

## Understanding the problem

V této části by člověk měl vědět, co je neznámá. Jaké na ni jsou kladeny podmínky. Dále zda podmínky jsou dostatečné, aby se jednoznačně proměnná dala určit. Jestli vůbec existuje způsob, jak podmínku splnit.

Jaká data jsou důležitá a jaká jsou zbytečná. Vyfiltrovat přebytečné konkrétnosti a zaměřit se pouze na abstraktní podstatu důležitou pro vyřešení problému.

Nakreslit si diagram zachycující tu abstraktní podstatu. Pojmenovat si proměnné ze zadání a nové pomocné proměnné pokud jsou užitečné.

Dokáži přepsat zadání úlohy do přesné matematické notace? Dokáží matematickou notaci ze zadání vysvětlit vlastními slovy?

Zde mi přijde na škodu, že toto sedí pouze na ten typ příkladů, kde se snažíme zjistit nějakou hodnotu. Např. musíme spočítat řešení nějaké rovnice. Nebo spočítat, kolik je nějakých objektů. Jak ale neznámou napasovat na příklad typu: vyvraťte nebo dokaže, najděte objekt splňující nějaké vlastnosti, kolik nejméně kroků je potřeba abychom něčeho docílili, navrhněte algoritmus

## Devising a plan

Zde člověk uvažuje o tom, jak problém vyřešit. Zamýšlí se nad tím, jestli už neviděl nějaký podobný problém. Tedy problém, který může jakožto konkrétní instance vypadat jinak, ale sdílí stejné abstraktní jádro.

Dále je dobré se zamyslet nad tím, jak by vypadala nějaká konkrétnější verze problému. Např. máme spočítat, jak dlouho trvá osmažit n topinek, ale místo toho si napřed zkusíme, kolik by to bylo pro konkrétní případ 3 topinek.

Hodí se zamyslet se také nad tím, jak by vypadal obecnější problém. To nám umožní detekovat, co je mezi naší konkrétní instancí a obecným probmémem sdílené. To co je sdílené je pak dost možná to důležité obecné abstraktní jádro problému.

V tomto momentu si také člověk může hrát s podmínkami, které musí řešení splňovat. Jak by se změnilo řešení, kdybychom nějakou podmínku změnili. Například její část úplně vypustili. Např. chceme zjistit, kolik existuje posloupností nul a jedniček takových, že neobsahují dvě jedničky bezprostředně vedle sebe. Můžeme uvolnit podmínku a nejprve se zamyslet, jaký je počet všech různých posloupností nul a jedniček. Nebo se zamyslet nad tím, jak by se řešení změnilo, kdyby ani nuly nemohly být bezprostředně vedle sebe. Tyto myšlenkové experimenty nám mohou poskytnout nový vhled do dané úlohy.

Vzali jsme v potaz všechny důležité skutečnosti, které jsme dostali v zadání. Například pokud řešíme nějakou úlohu se stromy (v teorii grafů), tak se ptát, zda jsme použili acykličnost stromů a to, že přidáním libovolné hrany vznikne cyklus. Použili jsme fakt, že odebráním hrany už by se strom znesouvislil? Vzali jsme v potaz skutečnost, že mezi každými dvěmi vrcholy existuje právě jedna cesta?

## Carrying out the plan

Nyní už jen provádíme to, co jsme si naplánovali v předchozí části. Nyní je důležité si zkontrolovat, zda v našem postupu od každého kroku k dalšímu dává přechod smysl. Zda ho dokážeme logicky odargumentovat a říci, proč funguje.

## Looking back

Je nyní výsledek očividný, když už ho máme před sebou? Dokážeme si výsledek nějak ověřit (experimentální program). Můžeme nějak výsledek omezit shora či zdola jednodušší úvahou a sedí nám výsledek do spočtených hranic? Např. pokud počítáme posloupnosti nul a jedniček jako výše, které zároveň musí ještě splňovat nějakou další vlastnost, tak nutně je horní mezí počtu takových posloupností počet všech posloupností nul a jedniček.

Ještě lepší je umět se zamyslet nad jiným způsobem, který by došel ke stejnému řešení. Pokud takový způsob existuje, tak nám může posloužit jako skvělá kontrola našeho předchozího výsledku.

Zároveň je pěkné se zamyslet nad tím, jestli nemůžeme výsledek ihned použít k řešení nějakého jiného problému.

# Purpose

Polya po zmínění čtyř metod výše navazuje kapitolou purpose neboli účel. Tedy za jakým cílem jako učitelé jdeme. Zmiňuje zde tyto body:

## Helping the student

Hlavní je, pomoci studentovi řešit matematické problémy. Avšak nejen vyřešit ten aktuální probíraný problém, ale nejlépe ho naučit řešit i další podobné problémy, na které student v budoucnu narazí.

Obecně chceme rozvinout studentovu dovednost nezávisle řešit problémy. Tedy řešit problémy s co možná nejméně externí pomoci. Zde je tedy důležité, aby především student přicházel na řešení těch problémů. Důležité je však, aby student nebyl ponechán problému úplně napospas. Učitel tedy musí pomáhat, ale jen v tom nejnutnějším a velice obezřetně.

Pomoci studentovi můžeme především tím, že budeme klást návodné otázky. Zde je klíčové, aby se učitel snažil co nejlépe vžít do role studenta. Tedy snažit se pomyslně číst studentovy myšlenky. Každá návodná otázka by měla být taková, že by si ji byl býval mohl pomyslet i samotný student. Tedy měla by odpovídat jeho aktuálním schopnostem a nanejvýš hraničit přesně s limited jeho dovedností.

## Questions, recommendations, mental operations

Hlavním účelem otázek je, abychom namířili studentovu pozornost na to nejdůležitější. Je to takový usměrňovač toku myšlenek na správný cíl. Polya uvádí seznam dobrých otázek, který ve finále koresponduje nepřímo se seznamem mentálních operací, které jsou užitečné pro řešení problémů. Snažil se je také setřídit v pořadí v jakém se nejpravděpodobněji člověku naskytnou.

## Obecnost

Nesnažíme se naučit studenta jedné konkrétní dovednosti. Tedy řešit jeden konkrétní problém. Chtěli bychom studenta naučit myšlenkovou šablonu, kterou dokáže aplikovat na celé spektrum problémů. Tedy to, co se student naučí by mělo být ideálně přenositelné i do jiných sfér života.

Autor však podotýká, že otázky se liší dle toho, zda je problém typu dokažte nebo nalezněte.

## Selský rozum

Otázky z autorova seznamu míří na to, aby byly prosté a jednoduše pochopitelné. Žádné komplexní divočiny. To, co je na tom seznamu zajímavé je to, že i když přece takové myšlenky používat občas můžeme, tak je většinou neformulujeme slovy a nekonáme ty postupy vědomě. No a to je škoda a toto se snaží autor prolomit.

## Teacher and student. Imitation and practice.

Student by si měl pozvolna uvědomit, jak moc jsou otázky ze seznamu užitečné. Tím, že mu budou pomáhat si nakonec zvykne si tyto otázky pokládat samostatně bez potřeby učitele.

Matematika je dovednost, kterou se člověk učí aktivně. Tedy tím, že aktivně imituje to, co už viděl a procvičuje to stále dokola.

Důležité je, že učitel by měl studenty hezky motivovat, aby problémy chtěli řešit!!! A hezky při řešení problémů dělat divadýlko!!!