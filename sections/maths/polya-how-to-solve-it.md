---
layout: default
title: "Polya: How to Solve it"
section_key: maths
date: 2025-09-13
permalink: /mathematics/polya-how-to-solve-it
---

# {{ page.title }}

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