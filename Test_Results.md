# Wyniki testów

## [TC-FUNC-001-APP-2](https://github.com/TO-perelki/testowanie/blob/main/LOW-LEVEL-TEST/LOW-LEVEL-TEST-APP.md#tc-func-001-app-2--weryfikacja-wyszukiwania-produktów-po-kodzie-kreskowym-produktów-nieistniejących-w-bazie)

**Rezultat:**
Po poprawnym zeskanowaniu kodu produktu nieznajdującego się w bazie, aplikacja wyświetla komunikat "Nieznany produkt", jednocześnie umożliwiając dodanie go do bazy produktów.

**Test zaliczony.**

---

## [TC-FUNC-002-APP-1](https://github.com/TO-perelki/testowanie/blob/main/LOW-LEVEL-TEST/LOW-LEVEL-TEST-APP.md#tc-func-002-app-1-weryfikacja-wyświetlania-szczegółowych-informacji-o-składnikach-produktu)

### Scenariusz: Produkt posiada uzupełnione szczegółowe informacje.
**Rezultat:**
Po poprawnym zeskanowaniu kodu produktu znajdującego się w bazie, użytkownik ma dostęp do szczegółowych informacji o składnikach każdego produktu.

**Test zaliczony.**

### Scenariusz: Produkt nie posiada uzupełnionych szczegółowych informacji.
**Rezultat:**
Po poprawnym zeskanowaniu kodu produktu znajdującego się w bazie, użytkownik nie ma dostępu do szczegółowych informacji o składnikach każdego produktu.

**Test zaliczony.**

---

## [TC-FUNC-004-APP-1](https://github.com/TO-perelki/testowanie/blob/main/LOW-LEVEL-TEST/LOW-LEVEL-TEST-APP.md#tc-func-004-app-1-weryfikacja-dodawania-nieistniejących-produktów-do-bazy-w-aplikacji-mobilnej)

**Rezultat:**
Po poprawnym zeskanowaniu kodu produktu nieznajdującego się w bazie, użytkownik może dodać go do bazy produktów. Po uzupełnieniu wymaganych informacji i zapisaniu dany produkt zostaje dodany do bazy, a po ponownym zeskanowaniu kodu pojawiają się informacje na jego temat.

**Test zaliczony.**

---

## [TC-FUNC-005-APP-1](https://github.com/TO-perelki/testowanie/blob/main/LOW-LEVEL-TEST/LOW-LEVEL-TEST-APP.md#tc-func-005-app-1--weryfikacja-wyświetlania-informacji-o-alergenach)

### Scenariusz: Produkt zawiera alergeny.
**Rezultat:**
Po poprawnym zeskanowaniu kodu produktu znajdującego się w bazie, użytkownik ma dostęp do informacji o alergenach produktu.

**Test zaliczony.**

### Scenariusz: Produkt nie zawiera alergenów.
**Rezultat:**
Po poprawnym zeskanowaniu kodu produktu znajdującego się w bazie, brak informacji o potencjalnych alergenach.

**Test zaliczony.**

---

## [TC-FUNC-006-APP-1](https://github.com/TO-perelki/testowanie/blob/main/LOW-LEVEL-TEST/LOW-LEVEL-TEST-APP.md#tc-func-006-app-1-weryfikacja-obsługi-wielu-języków-interfejsu)

**Rezultat:**
Po zmianie języka (tutaj angielski i polski) w ustawieniach aplikacji tekst interfejsu zostaje przetłumaczony na dany język.

**Test zaliczony.**

---

## [TC-FUNC-008-APP-1](https://github.com/TO-perelki/testowanie/blob/main/LOW-LEVEL-TEST/LOW-LEVEL-TEST-APP.md#tc-func-008-app-1-weryfikacja-wyświetlania-ocen-wartości-odżywczych)

**Rezultat:**
Po poprawnym zeskanowaniu kodu produktu znajdującego się w bazie, system wyświetla dane o wartościach odżywczych oraz wskaźniki zdrowotne.

**Test zaliczony.**

---

## [TC-FUNC-009-APP-1](https://github.com/TO-perelki/testowanie/blob/main/LOW-LEVEL-TEST/LOW-LEVEL-TEST-APP.md#tc-func-009-app-1-weryfikacja-obsługi-preferencji-dietetycznych-użytkownika)

**Rezultat:**
Po ustawieniu osobistych preferencji, produkty zostają oznaczone w zależności od dopasowania do wybranych preferencji żywieniowych.

**Test zaliczony.**

---

## [TC-FUNC-003-WEB-1](https://github.com/TO-perelki/testowanie/blob/main/LOW-LEVEL-TEST/LOW-LEVEL-TEST-WEB.md#tc-func-003-web-1-sortowanie-wyników-według-najczęściej-skanowanych-produktów)

**Rezultat:**
Po wybraniu z menu sortowania opcji "Najczęściej skanowane" produkty zostają posortowane według liczby skanowań w kolejności malejącej.

**Test zaliczony.**

---

## [TC-FUNC-003-WEB-2](https://github.com/TO-perelki/testowanie/blob/main/LOW-LEVEL-TEST/LOW-LEVEL-TEST-WEB.md#tc-func-003-web-2-sortowanie-wyników-według-nutri-score)

**Rezultat:**
Po wybraniu z menu sortowania opcji "Najczęściej skanowane" produkty zostają posortowane według liczby skanowań w kolejności malejącej.

**Test zaliczony.**

---

## [TC-FUNC-003-WEB-3](https://github.com/TO-perelki/testowanie/blob/main/LOW-LEVEL-TEST/LOW-LEVEL-TEST-WEB.md#tc-func-003-web-3-sortowanie-wyników-według-eco-score)

**Rezultat:**
Po wybraniu z menu sortowania opcji "Eco-Score" produkty zostają posortowane według wartości Eco-Score w kolejności rosnącej (od A do E).

**Test zaliczony.**
