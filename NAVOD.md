# Návod k aplikaci Fotoměření v4

**Fotoměření bylo vyvinuto pro měření obálky budov zvenku.** Vyfotografujte budovu zvenku a měřte její fasády, okna, dveře a další prvky obálky přímo na pořízených snímcích.Z fotografie můžete změřit délky, rozměry oken a dveří, plochy a úhly. Nejdříve aplikaci ukážete skutečně vodorovné a svislé hrany a zadáte známé rozměry. Teprve potom začnete měřit.

Návod platí pro [fotomereni-prototyp-v4.html](fotomereni-prototyp-v4.html). Ovládání a chování jsou popsané podle verze uložené v projektu k 6. 11. 2026.

## Rychlý postup

1. Otevřete HTML soubor aplikace v prohlížeči a upravte údaj **zakázka** vpravo nahoře.
2. V části **1 · Fotografie** vyberte snímek.
3. V části **2 · Kalibrace** ponechte **přesná – úběžníky (doporučeno)**.
4. Naklikejte nejméně dvě vodorovné a dvě svislé linie a stiskněte **Rektifikovat**.
5. Zadejte skutečný vodorovný a svislý rozměr a oba vyznačte po dvou bodech. Vyčkejte na stav **kalibrace aktivní (X i Y)**.
6. V části **3 · Měření** zvolte druh měření a naklikejte jeho body.
7. Zkontrolujte výsledky a stiskněte **Uložit projekt**.
8. Pro přenos výsledků stiskněte **Kopírovat tabulku (Excel)** a vložte je do tabulky pomocí Ctrl+V.

Podrobnosti jednotlivých kroků jsou níže. Pro první měření použijte dobře viditelnou rovnou stěnu a rozměry, které jste na místě skutečně změřili.

## 1. Příprava fotografie a rozměrů

Připravte si fotografii a alespoň jeden známý vodorovný a jeden svislý rozměr. Mohou patřit stejnému prvku, například šířce a výšce okna. Všechny rozměry budete zadávat v metrech: **120 cm = 1,2 m**, **20 cm = 0,2 m**.

Pro kalibraci vyberte dobře viditelné, co nejdelší hrany. Vhodné jsou nároží, parapety, nadpraží nebo vodorovný sokl. Malý referenční prvek a nepřesné kliknutí mohou způsobit velkou chybu při měření celé fasády.

Pracujte s jednou rovinou, například s jednou fasádou. Na nárožním snímku nekombinujte při kalibraci hrany dvou různě natočených stěn. Referenční rozměry mají ležet ve stejné rovině; zapuštěné či předsazené prvky mají vlastní korekci popsanou v oddílu 6.

Fotografie má obsahovat celé měřené prvky a rozeznatelné hrany. Zakryté rohy, rozmazání a výrazně šikmý záběr zhoršují spolehlivost výsledků. Známé rozměry ověřte měřením na místě; projektová dokumentace se může od skutečného provedení lišit.

## 2. Spuštění a načtení fotografie

1. Otevřete soubor **fotomereni-prototyp-v4.html** v internetovém prohlížeči. Aplikace funguje offline a nevyžaduje přihlášení.
2. Vpravo nahoře vyplňte **zakázka**. Pro odlišení snímků můžete použít například `DUM01-SZ`. Údaj se ukládá do projektu a používá se v názvu staženého souboru.
3. V části **1 · Fotografie** vyberte fotografii ze souboru, například JPG nebo PNG. Na počítači ji můžete také přetáhnout do velké pracovní plochy.
4. Kolečkem myši přibližte důležité hrany. Pro posun obrazu zvolte **Posun** a táhněte myší.

**Předvyplněná čísla jsou pouze příklady.** Aplikace začíná s číslem zakázky `10015`, měřítky `1.200` a `1.350` m a vzdáleností fotoaparátu `11.0` m. Použijte vlastní údaje. Vzdálenost fotoaparátu budete potřebovat při korekci zapuštění.

Po úpravě čísla přejděte klávesou Tab do dalšího pole, aby se změna projevila. Pokud číselné pole nepřijímá desetinnou čárku, zadejte desetinnou tečku, například `1.200`.

## 3. Doporučená kalibrace pomocí úběžníků

**Kalibrace** přiřadí fotografii skutečné rozměry. **Rektifikace** znamená narovnání perspektivy pro výpočet. Fotografie na obrazovce přitom zůstává zobrazená v původní perspektivě.

### Vodorovné a svislé linie

1. V části **2 · Kalibrace** ponechte možnost **přesná – úběžníky (doporučeno)**.
2. Stiskněte **+ vodorovná linie**. Klikněte na začátek a konec jedné hrany, která je ve skutečnosti vodorovná, například na hranu parapetu.
3. Stejným způsobem vyznačte druhou vodorovnou hranu. Volte dlouhé úseky rozložené po fasádě. Dobře viditelnou třetí linii můžete přidat stejným způsobem.
4. Stiskněte **+ svislá linie** a po dvou bodech vyznačte nejméně dvě skutečně svislé hrany, například obě nároží jedné fasády.
5. Počítadlo má ukazovat alespoň **2 H / 2 V**. Stiskněte **Rektifikovat**.

Vodorovnost a svislost posuzujte podle skutečné stavby. Kvůli perspektivě mohou tyto hrany na fotografii vypadat šikmo. Šikmá hrana střechy není vhodnou vodorovnou kalibrační linií.

Po úspěšné rektifikaci se pomocné linie skryjí. Znovu je zobrazíte stisknutím příslušného tlačítka **+ vodorovná linie** nebo **+ svislá linie**; jejich body pak můžete dotáhnout tažením.

### Skutečné měřítko os X a Y

1. Do číselného pole vedle **Měřítko vodorovné (2 body)** zadejte skutečnou vodorovnou délku v metrech.
2. Stiskněte toto tlačítko a klikněte na oba konce odpovídajícího rozměru ve fotografii. Například pro skutečnou šířku okna 1,2 m vyznačte právě tuto šířku.
3. Do pole vedle **Měřítko svislé (2 body)** zadejte skutečnou svislou délku.
4. Stiskněte toto tlačítko a klikněte na oba konce odpovídajícího svislého rozměru.
5. Zkontrolujte stav **kalibrace aktivní (X i Y)**. Samotné stisknutí tlačítka Rektifikovat ještě nestačí.

Obě měřítka musí být vyplněná a vyznačená. Po jejich dokončení se body skryjí; tlačítkem příslušného měřítka je můžete znovu zobrazit a upravit.

Před dalším měřením ověřte kalibraci na jiném známém rozměru, který jste pro ni nepoužili. Velká odchylka je důvodem zkontrolovat hrany, body, zadané jednotky a rovinu reference.

## 4. Rychlá kalibrace referenčním obdélníkem

Tuto alternativu použijte, pokud máte ve fotografii dobře viditelný obdélník se známou šířkou a výškou. Při měření rozměrů daleko za jeho hranicemi se více projeví chyba kliknutí.

1. Přepněte na **rychlá – referenční obdélník**.
2. Zadejte skutečnou **šířku ref. [m]** a **výšku [m]**.
3. Stiskněte **Klikat 4 rohy**.
4. Klikněte v tomto pořadí: **levý horní → pravý horní → pravý dolní → levý dolní**.
5. Stiskněte **Spočítat kalibraci** a ověřte výsledek na dalším známém rozměru.

Rohy lze v režimu **Klikat 4 rohy** upravit tažením. Použijte přesné hranice prvku, ke kterým patří zadané rozměry.

## 5. Měření délek, otvorů, ploch a úhlů

Po dokončení kalibrace vyberte v části **3 · Měření** příslušné tlačítko.

| Režim | Postup | Výsledek |
|---|---|---|
| **Vzdálenost (2 body)** | Klikněte na začátek a konec úseku. | Délka v metrech. |
| **Otvor (4 rohy)** | Klikněte levý horní, pravý horní, pravý dolní a levý dolní roh obdélníkového otvoru. | Šířka, výška a jejich součin jako plocha. |
| **Polygon** | Postupně klikejte po obvodu plochy. Po nejméně třech bodech stiskněte **Uzavřít polygon** nebo Enter. | Plocha a obvod. První bod není nutné klikat znovu. |
| **Sklon (2 body)** | Klikněte na dva body jedné šikmé hrany. | Její úhel vůči skutečné vodorovné ose kalibrované roviny a sklon v procentech. |
| **Úhel 2 linií (4 body)** | Nejprve dva body první linie, potom dva body druhé linie. | Menší úhel mezi liniemi, převedený do rozsahu 0–90°, a odpovídající procentní sklon. |

Měření ze dvou nebo čtyř bodů se dokončí automaticky. Polygon uzavřete tlačítkem nebo klávesou Enter. Při přepnutí režimu se nedokončené měření zruší.

Při umisťování a dotahování bodů pomáhá lupa s nitkovým křížem. U otvoru používejte hranice téhož prvku: například všechny čtyři rohy stavebního otvoru. Pro nepravidelnou plochu použijte Polygon.

Body polygonu veďte postupně po obvodu, aby se jeho hrany nekřížily. Pro čistou plochu fasády odečtěte plochy otvorů od plochy fasády při zpracování výsledků; aplikace eviduje každou plochu samostatně.

### Měření sklonu střechy

Kalibrujte štítovou stěnu a v režimu **Sklon (2 body)** označte šikmou hranu viditelnou ve štítu. Pro kontrolu můžete použít **Úhel 2 linií (4 body)**: první linii veďte po skutečně vodorovné hraně a druhou po stejné šikmé hraně.

**Oba body jedné linie musí ležet ve stejné rovině.** Nekombinujte například jeden bod na líci stěny a druhý na předsazeném okraji střechy. Linie na přesahu rovnoběžném s kalibrovanou rovinou může mít správný úhel bez korekce hloubky; údaj `d` úhly nemění.

Výsledky úhlů jsou v rozsahu **0–90°**. Procentní sklon není totožný s úhlem ve stupních: například **45° odpovídá 100 %**. U téměř svislé linie může procentní údaj zůstat prázdný.

U režimu **Úhel 2 linií (4 body)** je procentní údaj přepočtem vzájemného úhlu těchto linií. Sklon vůči vodorovné rovině vyjadřuje tehdy, když jako první linii použijete skutečně vodorovnou hranu.

Aplikace měří úhly v kalibrované rovině. Obecný prostorový úhel ani sklon střešní roviny ustupující do hloubky z pohledu od okapu tímto postupem přímo nezměříte.

## 6. Korekce zapuštění

Korekci použijte pro měřený prvek, který leží před referenční rovinou nebo za ní a je s ní rovnoběžný. Nejdříve si určete, ke které rovině patří známé rozměry použité pro kalibraci.

1. V části **4 · Korekce zapuštění** zadejte **vzdálenost fotoaparátu D [m]** od referenční roviny.
2. V tabulce výsledků u konkrétního měření vyplňte **d [m]**:

| Poloha měřeného prvku vůči referenční rovině | Hodnota d |
|---|---|
| Ve stejné rovině | `0` |
| Za referenční rovinou, dál od fotoaparátu | Kladná, například `0.20` pro 20 cm |
| Před referenční rovinou, blíž fotoaparátu | Záporná, například `-0.20` pro 20 cm |

Pokud kalibrujete podle zapuštěného okna a měříte líc fasády před ním, fasáda má záporné `d`. Pokud je referencí líc fasády a měříte zapuštěný prvek za ním, má tento prvek kladné `d`.

Korigované výsledky jsou ve sloupcích označených hvězdičkou: **š\***, **v/L\*** a **A\***. Původní sloupce a popisky na fotografii zůstávají bez této korekce. U úhlů je `d` pouze poznámkou a korigované sloupce zobrazují pomlčku.

Korekce délky používá poměr `(D+d)/D`, korekce plochy jeho druhou mocninu. Například při `D = 10 m`, `d = 0,2 m` a odečtené délce `2 m` vyjde korigovaná délka `2,04 m`. Vzdálenost D musí být větší než nula; pro skutečnou korekci ji nenechávejte prázdnou.

## 7. Čtení a oprava výsledků

Každé hotové měření se objeví v části **5 · Výsledky**. Tabulka je širší než levý panel; další sloupce zobrazíte vodorovným posunutím tabulky.

| Sloupec | Význam |
|---|---|
| **označení** | Název měření. Výchozí názvy jako L1, O1, P1 nebo U1 můžete přepsat, například na `okno-01`. |
| **typ** | Vzdálenost, otvor, polygon, sklon nebo úhel. |
| **š [m]** | Šířka otvoru. |
| **v/L [m]** | Výška otvoru, délka úseku nebo obvod polygonu podle typu měření. |
| **A [m²]** | Plocha otvoru nebo polygonu. |
| **úhel [°]**, **sklon [%]** | Výsledky úhlových měření. |
| **d [m]** | Hloubka vůči referenční rovině. |
| **š\***, **v/L\***, **A\*** | Hodnoty po korekci zapuštění. |
| **×** na konci řádku | Odstranění tohoto měření. |

Chybně umístěný bod můžete dotáhnout tažením v příslušném režimu. Pro úpravu bodů vodorovných linií aktivujte **+ vodorovná linie**, pro body svislého měřítka **Měřítko svislé (2 body)** a podobně. Pro úpravu bodů hotového měření zvolte měřicí režim, nikoli Posun.

## 8. Uložení projektu a výsledků

### Projekt pro další práci

Stiskněte **Uložit projekt**. Prohlížeč stáhne soubor například `fotomereni-DUM01-SZ.json`. Obsahuje fotografii, kalibraci, hotová měření a jejich údaje. Před uložením dokončete právě rozkliknuté měření.

Pro pokračování otevřete aplikaci a stiskněte **Načíst projekt**. Vyberte uložený soubor JSON. Verze 4 umí načíst také projekt uložený ve v3.

**Práce se neukládá automaticky.** Před zavřením nebo obnovením stránky projekt stáhněte a ověřte, že soubor máte uložený.

### Výsledky do Excelu

1. Stiskněte **Kopírovat tabulku (Excel)**.
2. Vyčkejte na hlášení o zkopírování.
3. V Excelu vyberte cílovou buňku a stiskněte Ctrl+V.

Do schránky se kopíruje tabulka se sloupci oddělenými tabulátory a s desetinnou čárkou. Tento přenos obsahuje číselné výsledky, nikoli fotografii a kalibrační body. Pro uchování celé práce použijte také **Uložit projekt**.

## 9. Začátek měření další fotografie

**Pouhé načtení jiné fotografie nevymaže dosavadní body, kalibraci ani měření.** Pro další snímek začněte čistý projekt:

1. Uložte dosavadní práci tlačítkem **Uložit projekt**.
2. Otevřete HTML aplikace v nové kartě nebo obnovte stránku.
3. Zadejte označení nového snímku, například `DUM01-JZ`.
4. Načtěte novou fotografii a proveďte novou kalibraci.

Pro každou fotografii ukládejte samostatný projekt. Stejnou kalibraci nepřenášejte na jiný záběr.

## 10. Ovládání myší, klávesnicí a dotykem

| Akce | Ovládání |
|---|---|
| Přiblížení a oddálení | Kolečko myši nebo gesto dvěma prsty. |
| Posun obrazu na počítači | Režim **Posun** a tažení, prostřední tlačítko myši nebo mezerník + tažení. |
| Posun na dotykové obrazovce | Tažení jedním prstem po volné ploše fotografie. |
| Umístění bodu | Kliknutí nebo krátké ťuknutí. |
| Oprava polohy bodu | Tažení bodu v příslušném režimu. |
| Vrácení bodu | **↶ Zpět bod** nebo Backspace. V režimu měření bez rozpracovaných bodů odstraní poslední hotové měření. |
| Zrušení rozpracovaného měření | **✕ Zrušit** nebo Esc; hotové řádky tím nemažete. |
| Dokončení polygonu | **Uzavřít polygon** nebo Enter, po nejméně třech bodech. |

Klávesové zkratky se ignorují při psaní do číselného či textového pole. V takové situaci použijte tlačítka na pracovní ploše. Odstraněné hotové měření je potřeba znovu naklikat.

## 11. Řešení běžných potíží

| Potíž | Postup |
|---|---|
| Fotografie se nezobrazila. | Ověřte, že vybíráte obrazový soubor. Pokud jeho formát prohlížeč nezobrazí, použijte kopii fotografie ve formátu JPG nebo PNG. |
| **Rektifikovat** je neaktivní. | Přidejte alespoň dvě dokončené vodorovné a dvě dokončené svislé linie. Každá potřebuje dva body. |
| Zobrazuje se **degenerované linie** nebo **degenerované body**. | Zkontrolujte vybrané hrany či rohy, jejich pořadí a odlišení. Nevolte opakovaně tutéž linii ani body v jedné přímce. |
| Aplikace píše **Nejprve dokonči kalibraci.** | U přesné metody dokončete rektifikaci i obě měřítka. U rychlé metody stiskněte **Spočítat kalibraci**. |
| Pomocné linie nebo body měřítek zmizely. | Po dokončení se záměrně skrývají. Zobrazí je tlačítko odpovídajícího režimu. |
| Výsledky výrazně nesedí. | Ověřte metry místo centimetrů, skutečné rozměry reference, oba směry měřítka, rovinu prvků a případné zapuštění. Změřte jiný známý kontrolní rozměr. |
| Po změně fotografie zůstaly staré body. | Uložte předchozí práci a začněte novou kartu nebo obnovte stránku podle oddílu 9. |
| Kopírování tabulky selhalo. | Prohlížeč může blokovat přístup ke schránce. Zkontrolujte jeho oprávnění. Pokud kopírování nelze povolit, uložte alespoň projekt JSON; potřebné hodnoty lze přepsat z tabulky. |
| Backspace nebo Enter nereaguje. | Zkontrolujte, zda právě nepíšete do vstupního pole. Použijte tlačítka **Zpět bod**, **Zrušit** nebo **Uzavřít polygon**. |

Počet desetinných míst ve výsledku nevyjadřuje zaručenou přesnost měření. Výsledek vždy posuzujte podle kvality fotografie, kalibrace a nezávislého kontrolního rozměru.
