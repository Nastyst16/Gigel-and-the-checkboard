# Gigel-and-the-checkboard
Exercise 3 - Homework PCLP 1

Problema 3 - Gigel si tabla de sah

    Modularizam problema cu ajutorul headerului intitulat "function3.h"

        Incepem prin citirea dimensiunii tablei de sah si a elementelor acesteia.
        In cazul in care piesa se afla pe un patrat cu coordonatele de acceasi paritate
    inseamna ca se afla pe un patrat de culoare alba. Astfel, trebuie sa ne deplasam
    la stanga daca numarul e negativ, iar la dreapta daca e pozitiv. Iesirea din
    tabla de sah duce la teleportarea pe partea opusa. Prin utilizarea 
    unui while, scadem succesiv valoarea patratului cu dimensiunea tablei de sah
    pana cand aceasta este mai mica decat dimensiunea. Ulterior adunam valoarea ramasa
    cu coordonata "y_coord".

        In cazul in care piesa se afla pe un patrat cu coordonatele de paritate diferita
    inseamna ca se afla pe un patrat de culoare neagra. Folosim analog acelasi algoritm
    doar ca de data aceasta piesa de sah se deplaseaza in sus (daca numarul e negativ) 
    sau in jos (daca numarul e pozitiv).

        De a lungul deplasarii piesei de sah am monitorizat distanta parcursa de aceasta
    in variabila "distanta". care urmeaza apoi a fi afisata.
        In momentul in care piesa de sah a ajuns pe un patrat cu valoarea 0 sau a ajuns
    pe pozitia initiala, ne oprim. Stim coordonatele in care am ajuns prin intermediul
    variabilelor "x_coord" si "y_coord".
        Afisarea liniei: scadem dimensiunea tablei de sah cu x_coord,
    deoarece asa este numerotata tabla de sah (de jos in sus)
        Afisarea coloanei: trebuie sa afisam coordonatele asemenea unui tabel din excel.
    Astfel ne folosim de variabilele "sute" si "zeci". Cele doua while-uri (liniile 49-58)
    calculeaza astfel:  numarul de litere de la A la Z este de 26, iar daca y_coord
    depaseste 26*26, inseamna ca o sa avem afisare de 3 litere (exp ABW). Analog in continuare.
