## Despre

O bază de date cu autogările din România + altele (

## Baza de date

Stații : ks, Numes, Loc, Adr

Operatori : ko, Numop, Web, Loc, Adr


ko: cod operator
kr: cod ruta
ps: poziție stație în ruta
ks: cod stație
hm: ora si minutul pentru statia respectiva

primary key(ko,kr,ps)

    Ko  Kr  Ps  Ks  Hm
    6   1   1   47  7:00
    6   1   2   56  8:00
    6   2   1   47  12:00
    6   2   2   56  13:00
    6   3   1   56  10:00
    6   3   2   47  11:00

Am descris trei rute fictive ale operatorului 6 intre statiile 47 si 56

E nevoie de un cîmp ps (poziție stație în rută) ca sa ai ruta în ordinea corectă
Asta pentru ca nu te poti baza pe ora : exista curse de noapte

Operator A

    Dej     8:00  9:00
    Gherla  8:15  9:15
    Cluj    9:00  10:00

Rezulta liniile urmatoare

    Op=A  Ruta=1 Poz=1 St=Dej H=8:00
    Op=A  Ruta=2 Poz=1 St=Dej H=9:00
    Op=A  Ruta=1 Poz=2 St=Gherla H=8:15
    Op=A  Ruta=2 Poz=2 St=Gherla H=9:15
    Op=A  Ruta=1 Poz=3 St=Cluj H=9:00
    Op=A  Ruta=2 Poz=3 St=Cluj H=10:00


## TODO

* De facut ceva sa aiba logica!
