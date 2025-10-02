1. Bevezető
A "Vita Kötélhúzás" egy valós idejű, böngészőalapú webalkalmazás, amelynek célja, hogy interaktív és vizuális keretet biztosítson tanórai vagy baráti viták lebonyolításához. Az alkalmazás egy tanár/moderátor (Admin) által vezérelt vitát tesz lehetővé, ahol két fél ('A' és 'B') érvel, a közönség pedig szavaz.

Az alkalmazás két külön oldalból áll:
*admin.html*: A vita létrehozására és menedzselésére szolgáló felület.
*index.html*: A vitához való csatlakozásra szolgáló felület a vitázók és a nézők számára.

A háttérben a Google Firebase Realtime Database biztosítja az adatok valós idejű szinkronizációját a résztvevők között.

2. Használati Útmutató
A. A tanár/admin teendői
A vita elindítása és moderálása az admin feladata.
Előkészületek: Nyisd meg a admin.html fájlt a böngésződben.
Vita létrehozása:
A megjelenő felületen töltsd ki a három mezőt:
Vita Témája / Kérdés: A vita központi kérdése (pl. "Szükség van-e a házi feladatra?").
'A' oldal álláspontja: Az 'A' oldal által képviselt nézőpont (pl. "Igen, a gyakorlás elengedhetetlen.").
'B' oldal álláspontja: A 'B' oldal álláspontja (pl. "Nem, mert túlterheli a diákokat.").
Kattints a "Létrehozás" gombra.

Kódok megosztása:
A létrehozás után a felület átvált a játék képernyőre. A képernyő tetején megjelenik egy "Csatlakozási Kódok" doboz.
Három különböző kódot fogsz látni. Ezeket kell megosztanod a résztvevőkkel a "Másolás" gombok segítségével:
*'A' Vitázó Kódja*: Ezt add annak a diáknak/csapatnak, aki az 'A' oldalt képviseli. Ez a kód egyszer használható.
*'B' Vitázó Kódja*: Ezt add a 'B' oldalt képviselő diáknak/csapatnak. Ez is egyszer használható.
*Nézők Kódja*: Ezt add a többi diáknak, a közönségnek. Ezt a kódot korlátlan számú néző használhatja.
Fontos, hogy a diákoknak az index.html oldal linkjét küldd el, ahol ezeket a kódokat használni tudják.

Vita lebonyolítása:
Amint az 'A' és 'B' vitázó is csatlakozott, a játék automatikusan elindul.
A te felületed (mivel te vagy az admin) minden információt mutat: a kör állását, a szavazatok pontos számát, és te látod az ADMIN jelvényt is.
Amikor egy kör a szavazási fázisba ér, egyedül te fogod látni a "Kör lezárása és eredmény (Admin)" gombot. Kattints erre, amikor le akarod zárni a szavazást.
A gomb megnyomása után a rendszer kiértékeli a győztest, frissíti az állást, és elindítja a következő kört.

Játék vége: A játék automatikusan véget ér, amikor az egyik fél 3-mal több kört nyer, mint a másik. A felületen megjelenik a győztes.

B. A vitázók ('A' és 'B') teendői
Csatlakozás:
Nyisd meg a tanártól kapott index.html linket.
Írd be a neked szóló, egyedi kódot ('A' vagy 'B' vitázó kódja).
Kattints a "Csatlakozás" gombra.
Érvelés:
Amikor te következel, a képernyőn megjelenik egy nagy szövegdoboz.
Írd be az érvedet vagy a válaszodat, majd kattints az "Elküldés" gombra.
Várj, amíg a másik fél válaszol, majd a közönség szavaz, és az admin lezárja a kört.

C. A nézők teendői
Csatlakozás:
Nyisd meg a tanártól kapott index.html linket.
Írd be a nézőknek szóló kódot.
Kattints a "Csatlakozás" gombra.
Szavazás:
Figyeld a vitát. Miután mindkét vitázó elmondta az érvét, a te képernyődön megjelennek a szavazógombok.
Kattints arra a gombra, amelyik érvvel jobban egyetértesz.
Körönként csak egyszer szavazhatsz. A szavazatod után a gombok letiltásra kerülnek.
A szavazatok állását nem látod, csak az admin.
