Izveštaj:
Kalkulator
Ovaj projekat predstavlja jednostavan kalkulator koji omogućava izračunavanje aritmetičkih operacija nad brojevima.
Pokretanje
Pokretanje kalkulatora se vrši pomoću klase Start. Pokrenite program tako što ćete uneti izraze koje želite da izračunate. Za izlaz iz programa unesite "exit".
Funkcionalnosti
Kalkulator podržava sledeće aritmetičke operacije: sabiranje (+), oduzimanje (-), množenje (*) i deljenje (/). Može se izračunati izraz koji sadrži ove operacije i brojeve. Izrazi mogu biti celobrojni ili decimalni.
Ograničenja
Kalkulator trenutno ima nekoliko ograničenja i propusta koji treba da se uzmu u obzir:
1.	Metoda ToString treba preimenovati u toString kako bi pratila konvencije za nazive metoda u Javi.
2.	Metoda Calculate ne obrađuje slučaj u kojem ulazni izraz sadrži zagrade, tako da zagrade nisu prepoznate.
Testiranje
Kako bismo testirali ispravnost koda, sprovedimo sistemsko testiranje po metodi crne kutije koristeći nekoliko test slučajeva:
•	Testiranje osnovnih aritmetičkih operacija sa celim brojevima:
•	Ulaz: 3 + 2, očekivani izlaz: 5
•	Ulaz: 7 - 2, očekivani izlaz: 5
•	Testiranje sa negativnim celim brojevima:
•	Ulaz: -4 + 6, očekivani izlaz: 2
•	Ulaz: 10 - 3, očekivani izlaz: 7
•	Testiranje sa decimalnim brojevima:
•	Ulaz: 1.5 + 2.3, očekivani izlaz: 3.8
•	Ulaz: 4.9 - 0.7, očekivani izlaz: 4.2
•	Testiranje deljenja sa nulom:
•	Ulaz: 8 / 0, očekivani izlaz: Infinity
•	Ulaz: -9 / 0, očekivani izlaz: Infinity
•	Testiranje sa nevažećim karakterima:
•	Ulaz: 5 + x, očekivani izlaz: ERROR
•	Ulaz: 2 ^ 4, očekivani izlaz: ERROR



Kod ima ukupno 235 linija koda (LOC). Ciklomatska složenost metoda evaluateExpression iznosi 14, dok ciklomatska složenost metode Calculate iznosi 12.
Obavljena je statička analiza koda korišćenjem SonarLint alata, a pronađeni su sledeći code smell-ovi:
Za fajl Calculator.java:
1.	Na liniji 18, koloni 30, treba promeniti velika slova u mala slova kod naziva metode kako ne bi došlo do konflikta (clash-a).
2.	Na liniji 24, koloni 26, treba promeniti velika slova u mala slova kod naziva metode kako ne bi došlo do konflikta (clash-a).
3.	Na liniji 74, koloni 25, treba promeniti velika slova u mala slova kod naziva metode kako ne bi došlo do konflikta (clash-a).
4.	Na liniji 18, koloni 30, treba promeniti velika slova u mala slova kod naziva metode kako ne bi došlo do konflikta (clash-a).
5.	Na liniji 4, koloni 14, može se dodati privatni konstruktor da bi se sakrio implicitno javni konstruktor.
6.	Na liniji 183, koloni 13, kod je nepotreban i može se ukloniti(linija koda je nepotrebna jer se ne koristi ni u jednom delu koda,
a njeno prisustvo može dovesti do nepotrebnog povećanja složenosti i održavanja koda.
Za fajl Start.java:
1.	Na liniji 8, koloni 3, treba zameniti System.out sa logger objektom.
2.	Na liniji 19, koloni 5, treba zameniti System.out sa logger objektom.
3.	Na liniji 6, koloni 10, treba promeniti "Expression" u "expression".

