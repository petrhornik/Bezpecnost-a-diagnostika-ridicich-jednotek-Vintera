[Co dodělat ]: #
[nic ]: #


# Bezpečnost a diagnostika řídících jednotek

$${\color{#FFA500}E14 \space \color{Gold}S25 \space \color{#4682B4}A10 }$$

## Cíl
-   Studenti rozliší pojmy Safety a Security

1)Rozdíl mezi safety a security

-   Doplní a především propojí si dosavadní znalosti z této problematiky
-   A na příkladech vysvětlí řešení některý z častých problémů
-   Dále popíší příklady diagnostických prostředků z oblasti HW
-   A na konkrétní řídící jednotce popíší základní diagnostiku
-   Vysvětlí, jak se provádí u této řídící jednotky základní diagnostika SW
-   A uvedou příklady nejběžnější nástroje pro diagnostiku SW

## Ověření cílů

Bezpečnost a diagnostika řídících jednotek

1. Bezpečnost (safety) řídících systémů
2. Zabezpečení (security) řídících systémů
3. Příklady HW a SW diagnostických prostředků
4. Ukázka základní diagnostiky vybraných řídících jednotek

        Safety = soubor prostředků, nařízení, zákonů, podmínek, které mají ochránit před/zabránit úrazem/úmrtím člověka či poškození stroje
        
        - zákony, pravidla, zákl. pojmy <- musíme dodržet
        - Proškolení, poukázání na základní pojmy a pravidla, zákony
        - řešíme hlavně bezpečnost lidí
        - např.: v autě airbag, senzory, kamery, ABS <- veškerá výbava související s prevencí nárazu/nehody, 
                izolované nástroje při práci s elektronikou, robot má vyznačený urč. prostor 
                ve kterém se pochybuje atd.
        - dodržení safety má větší prioritu než jakýkoli stroj/výrobek bez ohledu na cenu
        -u PLCček exustují tzv. safety plc(žluté krabičky), nebo nějaké karty

        Security = snaha zabránit přístupu nežádaných osob do systému/zařízení a jakékoli manipulace s ním

        - např.: zabránit manipulaci s IP (síťovými kamerami) - přístup k tomu co kamera vídí, její zastavení, manipulace se záznamem
        - stalking přes nezabezpečené kamery, policie nesmí sledovat lidi přes kabery BEZ soudního příkazu
        - hybridní válka = 
        - sledování pohybu lidí pomocí čídel vlhkosti, CO2, teploty - může sloužit k vydírání (musíme předejít) - např. v politice
        - penetrační test = zkouší způsoby jak/pokud jde se dostat do sítě firmy, která si tento test objedná 
        - jak zabezpečit zařízení:      1) zamezit/zabezpečit přístup - heslo, 2FA, biometrika, přistupovat mohou jen konkrétní zař., dáz zař. do jiné sítě, social engineering
                                        2)
        

## Úlohy

### 1. Safety

1. Při zapojování některé z úloh sepište, jaká bezpečnostní opatření jste museli dodržovat.

    <details>
        <summary> :bulb: Tip: </summary>
            Zaměřte se na bezpečnost práce v elektrotechnice.
    </details>

2. Zkuste vyhledat alespoň dvě normy/zákony, zabývající se konstrukcí zařízení z hlediska Safety, nebo bezpečností práce.

3. Na příkladech vysvětlete pojem Safety.

> :key: **Safety**
>
> Ve spojení s průmyslem lze zjednodušeně říci, že se jedná o bezpečnost před úrazem, či úmrtím.
  K zajištění se používají ochranné pomůcky (rukavice, brýle,...), specializované zařízení, komponenty, řídící jednotky,... (stop tlačítko, proudový chránič, safety PLC,...), ale také předpisy a provozní řády (např. školní řád a řád učeben), školení, apod.

### 2. Security

1. U některé z úloh, kde byla řídící jednotka připojena k internetu, sepište možná rizika z hlediska IT security a ke každému riziku dohledejte možná ochranná opatření.

2. Zkuste vyhledat, jaká legislativa se zabývá IT security.

3. Na příkladech vysvětlete pojem Security.

> :key: **Security**
>
> Zjednodušeně lze říci, že se zabývá ochranou majetku pře krádeží, poškozením, kompromitací, apod. V případě fyzického majetku (tedy např. i serveru, kde jsou uložena důležitá data) se realizuje např. oplocením, uzamčením, kamerovými systémy, alarmy, apod. V případě softwaru a dat se používají firewally, antivirové programy, omezení přístupu (např. heslem, změnou portu, apod.).


### 3. Diagnostika řídící jednotky

V následujících úlohách navrhněte a ověřte postup, jak odhalit závadu. Nezapomeňte popsat i jaké diagnostické prostředky k tomu potřebujete, případně jak je nastavíte.

1. Kontrolky (a případný displej) na řídící jednotce nesvítí.
    - Navrhovaný postup:
    - Použité diagnostické prostředky:
    <details>
        <summary> :bulb: Tip: </summary>
        Zkontrolujte napájení. 
    </details>

2. Vše vypadá funkční, pouze podle popisu funkce zařízení, jedna kontrolka zjevně nesvítí.
    - Navrhovaný postup:
    - Použité diagnostické prostředky:
    <details>
        <summary> :bulb: Tip: </summary> 
        Zkontrolujte přívodní vodiče. 
    </details>

3. Kontrolky na řídící jednotce svítí (a případný displej ukazuje stav RUN), ale není žádná odezva na stisknutí ovládacích tlačítek.
    - Navrhovaný postup:
    - Použité diagnostické prostředky:
    <details>
        <summary> :bulb: Tip: </summary>
        Zkontrolujte zapojení a nastavení tlačítek. Často jsou tlačítka zapojena na společnou zem, tou je možné začít. 
    </details>

4. Po stisknutí tlačítka se sepne jiná kontrolka.
    - Navrhovaný postup:
    - Použité diagnostické prostředky:
    <details>
        <summary> :bulb: Tip: </summary> 
        Buď jsou prohozené v zapojení, nebo v programu. 
    </details>

5. Hardware je zapojený správně, přesto program nepracuje podle zadání.
    - Navrhovaný postup:
    - Použité diagnostické prostředky:
    <details>
        <summary> :bulb: Tip: </summary>
        Použijte softwarové ladící nástroje (debugger/krokování programu). Nejprve však rozhodněte, zda lze program ladit přímo na hardwaru, nebo v simulátoru.  
    </details>

> :key: **Simulátor**
>
> Program, který napodobuje chování řídící jednotky, pro kterou je vyvíjen software.
> Např. <a href="www.wokwi.com">Wokwi</a>, simulator PLC v programovacím prostředí Mosaic, apod.
> Podrobněji např. na 
> Simulation software. Online. In: Wikipedia: the free encyclopedia. San Francisco (CA): Wikimedia Foundation, 2024, 19 September 2024, at 09:30. Dostupné z: <a href="https://en.wikipedia.org/wiki/Simulation_software">https://en.wikipedia.org/wiki/Simulation_software</a>. [cit. 2024-12-07].
> kapitoly Simulační software, Programovatelné logické automaty.
</details>

> :key: **Debugger**
>
> Zjednodušeně lze říci, že se jedná se o ladící nástroj, sloužící pro vyhledávání chyb v logice programu. V případě řídících jednotek využívá buď simulátor, nebo samotný hardware (pokud je na to uzpůsoben) k odzkoušení programu. Mimo jiné umožňuje krokování, používání brakepointů, apod.
> Podrobněji např. na 
> Debugger. Online. In: Wikipedia: the free encyclopedia. San Francisco (CA): Wikimedia Foundation, 2024, 28. 4. 2022 v 21:27. Dostupné z: <a href="https://cs.wikipedia.org/wiki/Debugger">https://cs.wikipedia.org/wiki/Debugger</a>. [cit. 2024-12-07].

> :key: **Logické chyby**
>

6. Rozdělte se na týmy. Každý připravte zapojení a program, který odzkoušíte a popíšete jeho funkci. Poté udělejte několik závad a navrhněte postup, jak byste je detekovali a odstranili. Poté nechte druhý tým problémy vyřešit.




