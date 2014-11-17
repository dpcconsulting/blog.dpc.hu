---
title: "Hacktivity 2014, Budapest"
layout: post
author: gabor
---


Sok év után, idén először sikerült eljutnom a Hacktivity-re, Kelet-Közép Európa IT Biztonsági Konferenciájára, melynek idén októberben a MOM Kulturális Központ adott otthont. A Hacktivity az etikus hackerek, biztonsági tanácsadók és szakértők fóruma. Lelkes amatőr érdeklődőként látogattam ki a rendezvényre. Számtalan könyvet, cikket elolvastam már a témával kapcsolatban, gyakorlatom nincs, tehát kíváncsi voltam.

A rendezvény fő mondanivalóit annak rendje és módja szerint a két napos rendezvény két keynote előadása hordozta magában: mire kell figyelnünk a mai világban a biztonság tekintetében, milyen új kihívásokkal kell szembenéznűnk, legyünk akár felhasználók, fejlesztők, biztonsági szakértők.


Keynote előadások

**Jason Chan**
**Keynote - Építsünk üvegházat: modern szoftver architektúrák és gyakorlatok biztonsági adaptációi**

A mai szoftverek hatalmas átalakuláson mennek keresztül, tekintve az infrastruktúrát, az üzemeltetést, sőt, még a szoftverfejlesztés módszertana is gyökeres megváltozott. A tradícionális vízesés modellt kiszorítják az agilis módszerek, megjelennek a mikroszervizek a monolitikus (makro)rendszerekkel szemben, egyre több és több szolgáltatás jelenik meg felhő alapokon, egyre nagyobb figyelmet kap a *DevOps*.

*Ami az alkalmazások biztonságát illeti, ideje gyászolni: viszlát traditionalis alkalmazás biztonság, alig ismertünk, nem sok időt töltöttél velünk.*

Új feladatok várnak ránk, új problémákkal találjuk magunkat szemben, ugyanis a jól bevált tervezési mintákat és a tradícionális biztonsági modelleket nyugodtan elfelejthetjük. Egy folyamatosan változó rendszerben újabb és újabb biztonsági problémák lépnek fel, amelyekhez nehéz idomulni, folyamatos nyomonkövetést igényel, hogy időben be tudjunk avatkozni. Egy ilyen rendszer esetében nem tudunk egyetlen egzakt szabályrendszert, modellt, védelmi protokollt felépíteni, amely hatásos és gyorsan képes reagálni. Új technikák és eszközök szükségesek, amelyek minden törvényszerűségtől mentesek, csupán irányelveket és paradigmákat tartalmazhatnak. 

Mi a teendő ezután? 
Mindenek előtt ismernünk kell a környezetet, amivel dolgozunk. A hangsúly ennek a változó környezetnek a folyamatos karbantartásán, monitorozásán van, és az ezekből valamilyen metrikahalmaz által meghatározott, tesztelés útján kinyert adatokon. Az agilis módszertanhoz hasonlóan, itt is nagyon fontos, minél hamarabb legyen visszacsatolásunk a rendszer állapotát illetően, jelen esetben biztonsági szemmel nézve: a tesztek elvégzése után az ezekből készített rengeteg riport segítségével feltárhatjuk a rendszer sérülékeny pontjait.
A folyamatot az előadó által megadott sémában tudunk követni: discover, inventory, test, report.
Jason Chan a Netflix által fejlesztett, nyílt forráskódú *Security Monkey* eszköz segítségével a fent említett sémában kínálja a megoldást rendszerünk biztonságának megőrzése érdekében. Zárszóként az egyik legfontosabb irányelv, amely a biztonsági kérdésekben igen komoly hibaforrás: *Next, tomorrow, later versus now.*


**David Jacoby - IOT: HOGYAN TÖRTEM FEL A LAKÁSOM**

David Jacoby Vezető biztonsági kutató, Skandináv Régió, Globális Kutató és Elemző Csoport
David 2010-ben csatlakozott a Kaspersky Lab-hez mint a skandináv régió és a Benelux államok vezető biztonsági kutatója.
[https://hacktivity.com/hu/hacktivity-2014/eloadok/david-jacoby/](https://hacktivity.com/hu/hacktivity-2014/eloadok/david-jacoby/)

Egyértelműen hatásos és tanulságos prezentációnak lehettünk szem- és fültanúi a szombat reggeli nyitó előadáson, amelyen David elmesélte, hogyan hackelte meg a saját otthonát. David Jacoby azt a feladatot kapta, tesztelje saját otthonának biztonságát, mennyire szenzitív és sérülékeny az a hely, ahol él, egyszóval feltörte saját otthonát. Az eredmény megdöbbentő, ugyanis nem arra fektette a hangsúlyt, hogyan csinálta, sokkal inkább arra, hogy miért, és félelemre ad okot az a tény, hogy milyen könnyen. 3 hónapot töltött azzal hogy feltörje az otthonában található kütyüket. Ezalatt sikerült meghackelnie a NAS adattárolóját, hálózati routerét, nyomtatóját. Az okostévéjének a képernyőjére kirakott egy képet, Borat mosolyog rajta. Elmondása szerint azért volt könnyű dolga Davidnek, mert az elektronikai eszközei kivétel nélkül csatlakoztatva vannak az otthoni hálózatra. Mindannyiunkban felmerül a kérdés, hogy egy blu-ray lejátszónak mi szüksége van internet kapcsolatra, illetve az otthoni fájlszerverünk miért érhető el a világhálóról.

A mindenki által szajkózott "rohanó világ”, mára már dogmává vált mondása itt is megfigyelhető. Rohanunk előre, mindig egyre újabb és újabb termékek jönnek ki a piacra, amit tegnap vásároltam holnapra elavul, és a gyártók kontójára írható fel, hogy a régebbi termékekre (a tegnapira) már nem jön ki újabb és újabb biztonsági frissítés. A kereskedelemből ismert time-to-market kifejezésből a time egyenlő a “Holnapra” mondattal, ezáltal rengeteg hibás, biztonságilag szempontból tragikusnak mondható termék. Percről percre állítják le x típus gyártását, y gyártását kezdik el, z terméket nem fejlesztik tovább, stb. Az már mellékes, hogy a legtöbb esetben nem is értesülünk ezekről, külön vadászni kell a hálózaton, hogy jön-e még ki új frissítés kedvenc okos kütyünkre vagy sem.
David meg is jegyezte: mikor felhívta egy pár biztonsági résre a figyelmet egy-két gyártónál, általában kétféle választ kapott: az egyik, hogy nálunk nincsenek biztonsági rések, nyilván az eszköz tökéletes, a másik, ez a megdöbbentőbb, az már régi, mármint a 6 hónapos termékre.

*A 6 hónap az régi, mégis milyen időközönként vegyek tv-t?*

Tehát a gyártók hozzáállása problémát okoz, nem csak szoftveresen lehet bejutni az eszközre hanem hardverhibákból származó biztonsági réseken keresztül is.
Hemzseg a piac az olyan kütyüktől, amelyek gyárilag rosszul vannak, vagy leginkább sehogy sincsen beállítva. A legtöbb eszköz mindenféle felhasználónév jelszó pár nélkül elérhető, hozzáférhetőek az esetleg rajta beállított ügyfél adatok, példának okáért egy hálózati modem és/vagy router esetében. *Minden eszköz, amely rendelkezik hálózati interfésszel, sebezhető.* Az előadáson mutatott olyan böngészőből elérhető konfigurációs felületet, hogy a bal oldali menüben elérhető volt két elem, a harmadik nyitva volt a jobb oldalon, mint tartalom, és csak idők múlva esik le egyébként hogy eredetileg a menü három pontból áll. Nem éppen a legtámadhatóbb pontja a programnak, de tény, hogy defektes, és minősíti is a terméket, leginkább a gagyi kategóriába sorolható.

Ugyanolyan hibás a felhasználó is, a felhasználó sem fordít elég időt és energiát a saját otthoni biztonsági beálllításaira. Ez lehet idő hiánya, lustaság, nem megfelelő szaktudás hiánya, nem megfelelő segítségkérés hiánya. Az esetek megdöbbentően nagy százalékában az internetről elővarázsolt hálózati kütyü alapértelmezett felhasználónév jelszó párosa elegendő a bejutáshoz. Nyilván az a felhasználó, aki még arra is lusta, hogy a gyári alap jelszót megváltoztassa, nem fogja a további beállításokat sem elvégezni, az, aki a mai napig nem érti, mi szükség van a jelszó használatára, azzal nem lehet mit kezdeni.

További példa beállításokra, amelyet David is hangsúlyozott, az az eszköz amelynek feltétlenül nem kéne, hogy elérje az internetet, például egy fájlszerver vagy NAS szerver, amelyen a családi fotóalbumot tároljuk, lehetne egy másik hálózaton, egy másik szegmensen. Ez nyilván már komolyabb beállításokat, szakértelmet, komolyabb időbefektetést igényel, amelyre már nem minden felhasználónak van lehetősége, és nyilván nem is várható el a felhasználótól, és így akaratukon kívűl válhatnak sebezhetővé. 

A megoldás
A tudomány mai állása szerint nincs: egész egyszerűen nem lehet mondani egy egzakt megoldás a problémára, mert nem lehet az ellenőrzésünk alatt tartani saját kis kütyüjeinket. David szerint egy nagyobb kontrolra lesz szükség az otthoni hátózatunk felett, mely nagyon nagy valószínűséggel valamilyen magasabb szintű biztonsági szoftverben fog manifesztálódni. Egyelőre ismeretterjesztő anyagok terjesztésével, beállításokban való segítségnyújtással, és a felhasználók hozzáállásának változtatásával lehetne növelni a védelmet: A gyártók és szakemberek annyiban lehetnek a segítségünkre, hogy megfelelő használati útmutatóval, kellő mennyiségű információval látják el a készüléket. Felhasználóként meg igenis tessék odafigyelni legalább arra, hogy az alapértelmezett jelszót meg kell változtatni, továbbá ne legyünk lusták átolvasni, értelmezni, beállítani, és ha nem megy, akkor segítséget kérni, és el kell felejteni a "a drágább az biztos jobb is” elvet.



**eXploitable Markup Language**

Mivel rengeteg helyen találkozunk az XML-lel közvetve vagy közvetlenül, rengeteg technológia épül rá, alapjául szolgálhat kommunikációs protokolloknak, esetleg elrejtve titokban beágyazottan használjuk, (és még a végtelenségig sorolhatnám,) érdemes volt megnézni a róla szóló, nevében is kifejező előadást: eXploitable Markup Language. 
Az előadók szerint: *Az XML feldolgozókat érintő támadási formák ősidők óta ismertek, ennek ellenére tapasztalatunk szerint még mindig nem kapnak elég figyelmet.*
Igaz, hogy az előadás elején viccesen leszögezték, hogy főleg nem webes XML támadásokról lesz szó, az első néhány demo mégis ebbe a kategóriában futott, hogy megismerhessük XML fájljainkban rejlő gyengeségeket. Egy gyakorlat-orientált előadás keretei között minden egyes rövid elméleti kérdés, egy-egy ötlet egy célzott, a való életből vett példán egy PoC programmal volt végvezetve és bemutatva. 
A webes példákon keresztül megismerhettük, hogyan kell belecsempészni XML állományokba úgy kódrészeket, hogy azok meg is hívódjanak. Ezt követően a való életből egy példát említenék: az egyik, ami nagyon elnyerte a tetszésem az az volt, hogyan lehet egy Visual Studio Project megnyitásával eljutni egy távoli asztal kapcsolathoz, és léphetünk be adminisztrátori jogosultságokkal. Elég összetettnek éreztem, rengeteg csillag-együttállásnak kell stimmelnie ugyan, de láthattunk példát arra, hogyan kell egy víruskeresővel ellátott mail szerverről, egy bizonyos víruskereső egy hibájából fakadóan, továbbjutni és átvenni az irányítást az azonos hálózaton lévő szerveren XML alapú attachment segítségével.
A rengeteg demoval egy hasznos, szórakoztató előadást láthattam. Aki a bővebb technikai részletek iránt érdeklődne, hogyan kell felkészülni az ilyen és hasonló támadások ellen, annak az XXE témakörben való elmélyülést javaslom. 


**Kémelhárítás**

A sajtóban is tárgyalt, nemzetbiztonsági körökben előszeretettel használt *FinSpy* Androidos kémprogram működése is terítékre került Marosi Attila előadásában.

Az előadó bemutatóként a nagyérdemű előtt telepítette a kémprogramot, majd bemutatott pár konfigurációs lépést, mely eseményekre figyeljen az alkalmazás, hogy a program a megfelelő pillanatokban aktivizálódhasson. Így például láthattuk, hogyan lehet kiolvasni a telefonkönyvet, illetve hogyan lehet a telefonra érkező hívást átírányítani, és lehallgatni a készüléket.
A kémprogramot nemzetbiztonsági szervek is használják, ennek ellenére a program titkosítás szempontjából korántsem mondható erősnek: 
A kulcs egy mai átlagos számítógéppel alig másfél nap alatt visszafejthető, ennek megléte nem is feltétlen szükséges, és a konfigurációs fájl is csak az x-edik verzióban kapott kulcsos védelmet.

Megtudtuk, ha IMEI számunk van, mindenünk van: ha nem is mindenre, de sok mindenre elég, elég lehet. A sors ironiájának is felróható, hogy ez a számsor, még szerencse :), megtalálható a telefonunkon. A kémprogram a titkosított csatornán természetesen ezt az információt is továbbítja a szerver felé. A program egyébiránt tartalmaz kisebb-nagyobb késleltetéseket, hogy ne tűnjön fel a megnövekedett adatforgalom, erőforráshasználat.

Megtudtuk, hogy kémprogrammal fertőzött telefonunk SMS segítségével konfigurálható, és ha ez még nem lenne elég, ráadásként ehhez például nem szükséges a kulcs ismerete. Az üzenetek elnyelődnek, tehát a tulajdonos tudomást sem vesz arról, hogy a figyelem középpontjában áll.




**Intermezzo**

Feladatok, játékok, érdekességek - 
A rendezvény egyes helyszíneire, például a szervezőknek, VIP vendégeknek, sajtóképviselőknek stb, csak megfelelő színű karszalaggal, STAFF feliratú polóval, bármilyen hasonló igazolvánnyal lehetséges a belépés. Korábbi konferenciák alkalmával, lévén ez egy biztonság-technikai fesztivál, igen, ezekre a helyekre be kellett jutni, kellett csinálni bent egy fotót, vagy bármilyen módon bizonyítani kellett, hogy bent volt az illető, és ezért különböző értékes tárgynyeremények jártak. Mivel nem találtam semmilyen ráutaló jelet, a feladatról megfelelő reklámot, nem hallottam pletykát, nem kockáztattam. A kérdőív kitöltések mellett, amelyek az e-mail címünk megszerzéséért és későbbi hírlevelekért léteznek, vannak izgalmas játékok is, amelyeknek akár további állomásai is lehetnek. Én is tollat ragadtam és kitöltöttem egy játékot, ahol egy security log-ból kellett a kérdésekre a megfelelő választ kikeresni egy szuper baseball sapkáért(Y). A 24 órás versenyre azért nem neveztem, mert nekem biztos, hogy egy ici-picivel több időre lett volna szükségem. :)

**Hasznos mondások**

*Hosszasan töprenghetünk azon, van-e merszünk felcsatlakoznunk a rendezvény WIFI hálózatára.*

*a promóciós névjegykártyákon szereplő QR kódot van-e bátorságunk okostelefonunkkal beolvastatni*

*a redundancia lényege, hogy több helyről lehet ellopni ugyanazt az adatot*


**Android**

A második napon több előadás foglalkozott az okostelefonok, főleg az Android támadhatóságával.

Sokakat mozgat a kérdés, az okostelefonok világában mennyire érezhetjük magunkat biztonságban, mire kell, kellene odafigyelnünk, milyen új veszélyek leselkednek ránk, és mit tud tenni akár a biztonsági szakértő, akár a felhasználó, akár a fejlesztő. Régen is lehetett ilyet, csak kicsit nehezebben, tartja a szóbeszéd. Manapság se könnyű, de az eszközkészletet tekintve jóval szélesebb a paletta.

A probléma
Milyen kérdések merülnek fel egy Androidos alkalmazás telepítése közben.
Egy apk letöltése és telepítése során a telefonunk különböző jogosultságokat kér tőlünk, engedélyt kér az alkalmazás mihez férhet hozzá, és ha valamivel esetleg nem egyeznénk bele, akkor megszakítjuk a folyamatot. Joggal merül fel bennünk a kérdés, hogy egy *zseblámpa* programnak mi szüksége van internet-hozzáférésre, miért kérdezi meg identitásunkat, továbbmegyek, mégis mi kell neki a telefonkönyvből? GPS lokációra is sűrűn látunk feleslegesnek tűnő példát: biztos lekérdezik, hol használtam a zseblámpát, és legközelebb oda telepítenek közvilágítást. Továbbgondolva a problémát: valóban csak azt teszi az alkalmazás, amire engedélyt adtunk, vagy éppen most kerülünk be a következő adatbázisba?

A biztonsági szakemberek elemzőprogramok segítségével keresik a választ: milyen veszélyes, kártékony kódokat tartalmaznak az egyes alkalmazások funkciói, milyen adatokat továbbít rólunk a rendszer, és még sorolhatnám.

Napjaink nehézségei - 
Tegyük fel, hogy szeretnék egyes kódrészleteket tömöríteni és/vagy elrejteni. Ebben nyújtanak segítséget a packerek. *A packer a definíciója szerint olyan csomagolóprogram, mely a szoftver egyes részeinek tartalmát tömöríti és/vagy elrejti.* Kíváló megoldást kínál azon emberek számára, akik kártevő kódrészleteket, a 90-es évek "termékeként" ismert malware-eket rejtenek el saját alkalmazásukban, vagy mások által publikált, megbízható alkalmazásokban, amelyeket feltörtek, és továbbadtak.

Ebben az esetben a legismertebb elemző programunkat az *apktool*t nyugodtan kidobhatjuk. 
A *Separating from Packers* előadáson a következő packereket tárgyalta az előadó: Pangxie􏰀, LIAPP,􏰀 Bangcle,􏰀 ApkProtect. Pár elméleti kérdés tisztázása után, a felsorolt packerek közül kettőt "éles környezetben" bemutatott, hogyan kell a packer segítségével becsomagolt alkalmazásokat visszafejteni.
Az előadásban tárgyalt packer-ek - a Bangcle és az ApkProtect - a DEX fájlokban levő titkosított kódokat használják, melyeket az alkalmazás az osztott könyvtárakban található natív kódot felhasználva tölt le futásidőben, tehát pusztán a fejlesztés megkönnyítésére szánt emulátor memóriájában megkereste azt a memóriaterületet ahol az alkalmazásunk található, és onnan kiolvasta és visszafejtette a tikosított obfuszkált forráskódot.
Ezek szerint a "Mire is jó valójában az Android Emulátor?" kérdésre a válasz attól függ, melyik konferencián ülünk éppen (developer tool vs hacking tool).

Másik nagy probléma az alkalmazás kommunikációja a külvilág felé, milyen adatokat szolgáltatunk, küldözgetünk szerte a világba a tudtunk nélkül.
Megoldás lehet a telefonunk route-olása, vagy egy tűzfallal megtámogatott számítogépre való proxy-zás, de a blackbox féle tesztelést *a vagtában való lövöldözéshez* hasonlította a két penteszter, akik a következő előadást tartották a Android témában: *Advanced tracing and monitoring*.
A megoldás lényege:
A VM-be bytekódszinten a függvények belépési és kilépési pontjain a paramétereket kiolvassák, és az Android log API-jának segítségével kiírják az eredményeket. A Python-t azért szereti mindenki, mert tömör, gyorsan lehet benne algoritmusokat, megvalósításokat kipróbálni, és mindez meg van fejelve azzal, hogy már meg van benne írva minden. Itt is láthatuk a hatékonyságát, pár apró kis script segítségével összeraktak előttünk egy debugger, elnevezésükben deLogger nevű programot, mely név hűen tükrözi, mit csinál valójában a program. Nem több mint öt-hat kattintás meg egy-két input mező kitöltésével igen hamar létre lehet hozni megabájtos fájlokat, így hát célszerű a számunkra releváns kódrészletek feltárására koncentrálnunk, ha elemzünk egy Androidos alkalmazást.

A lehetőségek tárháza dinamikus idejű megoldásokra is kiterjed. Stílusos címválasztással, a *Beoltjuk az Androidot* című előadáson bemutattak egy Vaccine névre hallgató programot, amely futási idejű elemzést, beavatkozást, manipulációt tesz lehetővé: *egy kis kódot beszúrunk az APK-ba, majd kapcsolódunk hozzá és a Java Reflection felhasználásával futási környezetben módosítjuk az értéket, a hívási metódusokat, a nem biztonságos osztályokat és a feladatok automatizálására saját szkripteket hozunk létre*. 
Csodálatos volt látni, hogy az *apk* kódjának megváltoztatása nélkül hogyan lehet kisebb-nagyobb változtatásokat eszközölni akár egy egyszerű kis táblás játékon.


**Summary**

Azon túl, hogy rengeteg érdekes, meghökkentő, olykor vicces demo segítségével temérdek hogyan kérdésre kaptunk választ, a fő mondanivaló igenis az, hogy nem törődünk eleget az otthonunkat érintő biztonsági kérdésekkel, gyártói oldalról még ráadásul akadályoztatva vagyunk. Létezik megoldás, ez pedig az idő. Kellő ráfordítással igenis lehet tenni a rosszindulatú behatolások ellen, nem szabad sajnálni az energiát, ugyanis a ráfordított idő nem mutat a végtelenbe, és még most neki kell állni a feladatnak, mikor még nem késő.

gabor



