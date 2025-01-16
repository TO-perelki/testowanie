# Wyniki testów funkcjonalnych i niefunkcjonalnych

## [TC-FUNC-003-WEB-1](https://github.com/TO-perelki/testowanie/blob/main/LOW-LEVEL-TEST/LOW-LEVEL-TEST-WEB.md#tc-func-003-web-1)
**Rezultat:**  
Wyniki wyszukiwania są posortowane według liczby skanowań w kolejności malejącej - **test zaliczony**

---

## [TC-FUNC-003-WEB-2](https://github.com/TO-perelki/testowanie/blob/main/LOW-LEVEL-TEST/LOW-LEVEL-TEST-WEB.md#tc-func-003-web-2)
**Rezultat:**  
Wyniki wyszukiwania są posortowane według wartości Nutri-Score w kolejności rosnącej (od A do E) - **test zaliczony**

---

## [TC-FUNC-003-WEB-3](https://github.com/TO-perelki/testowanie/blob/main/LOW-LEVEL-TEST/LOW-LEVEL-TEST-WEB.md#tc-func-003-web-3)
**Rezultat:**  
Strona nie ładuje się poprawnie, wyświetlany jest następujący komunikat:  
*Software error:  
MongoDB::DatabaseError: multiplanner encountered a failure while selecting best plan :: caused by :: operation exceeded time limit  
For help, please send mail to the webmaster (contact@openfoodfacts.org), giving this error message and the time and date of the error.* - **test niezaliczony**

---

## [TC-FUNC-004-WEB-2](https://github.com/TO-perelki/testowanie/blob/main/LOW-LEVEL-TEST/LOW-LEVEL-TEST-WEB.md#tc-func-004-web-2)
**Rezultat:**  
System wyświetla informacje na temat produktu, z możliwością ich edycji.  
Produkt nie zostaje dodany ponownie. - **test zaliczony**

---

## [TC-FUNC-004-WEB-3](https://github.com/TO-perelki/testowanie/blob/main/LOW-LEVEL-TEST/LOW-LEVEL-TEST-WEB.md#tc-func-004-web-3)
**Rezultat:**  
System nie pozwala dodać zdjęcia bez kodu kreskowego, ale w trakcie dodawania takiego zdjęcia wyświetla się komunikat:  
*Upload error*  
a w samej konsoli pojawia się błąd:  
`POST https://world.openfoodfacts.org/cgi/product.pl 500 (Internal Server Error)`.  
Oczekiwanym wynikiem byłoby wyświetlenie komunikatu o braku kodu kreskowego w obrazie.  - **test niezaliczony**

---

## [TC-FUNC-005-WEB-1](https://github.com/TO-perelki/testowanie/blob/main/LOW-LEVEL-TEST/LOW-LEVEL-TEST-WEB.md#tc-func-005-web-1)
**Rezultat:**  
Po wybraniu alergenów system pokazuje produkty, nie zawierające ich lub pokazuje informacje, że nie ma danych o alergenach - **test zaliczony**

---

## [TC-FUNC-007-WEB-1](https://github.com/TO-perelki/testowanie/blob/main/LOW-LEVEL-TEST/LOW-LEVEL-TEST-WEB.md#tc-func-007-web-1)
**Rezultat:**  
Zgłoszenie jest wysyłane i widoczny jest komunikat potwierdzający *"Changes saved"*. - **test zaliczony**

---

## [TC-FUNC-008-WEB-1](https://github.com/TO-perelki/testowanie/blob/main/LOW-LEVEL-TEST/LOW-LEVEL-TEST-WEB.md#tc-func-008-web-1)
**Rezultat:**  
Wyświetlane są poprawne dane o wartościach odżywczych oraz wskaźniki zdrowotne (np. Nutri-Score). - **test zaliczony**

---

## [TC-FUNC-009-WEB-1](https://github.com/TO-perelki/testowanie/blob/main/LOW-LEVEL-TEST/LOW-LEVEL-TEST-WEB.md#tc-func-009-web-1)
**Rezultat:**  
Produkty są oznaczone według dopasowania z preferencjami użytkownika. - **test zaliczony**

---

## [TC-NFUNC-001-WEB-1](https://github.com/TO-perelki/testowanie/blob/main/LOW-LEVEL-TEST/LOW-LEVEL-TEST-WEB.md#tc-nfunc-001-web-1)
**Rezultat:**  
Czas oczekiwania na wyświetlenie wyników wyniósł mniej niż 2 sekundy - **test zaliczony**
