# Przypadki Testowe dla Aplikacji Webowej

## TC-FUNC-002-WEB-1: Weryfikacja wyświetlania szczegółowych informacji o składnikach produktu

**Cel:** Sprawdzić, czy użytkownik ma dostęp do szczegółowych informacji o składnikach każdego produktu.  

**Warunki wstępne:**
- Strona dostępna pod adresem: https://world.openfoodfacts.org 
- Produkt istnieje w bazie danych.

**Kroki:**
1. Wyszukaj produkt na stronie, używając "Search a product".
2. Otwórz szczegóły produktu.

**Oczekiwane wyniki:**
- Wyświetlane są szczegółowe informacje o składnikach produktu, w tym ich ilości, pochodzenie i wartości odżywcze.

---

## TC-FUNC-003-WEB-1: Sortowanie wyników według najczęściej skanowanych produktów

**Cel:** Zweryfikować, czy system sortuje wyniki wyszukiwania według najczęściej skanowanych produktów.  

**Warunki wstępne:**
- Strona dostępna pod adresem: https://world.openfoodfacts.org 

**Kroki:**
1. Wyszukaj dowolną kategorię produktów na stronie.
2. Z menu sortowania wybierz opcję "Najczęściej skanowane".

**Oczekiwane wyniki:**
- Wyniki wyszukiwania są posortowane według liczby skanowań w kolejności malejącej.

---

## TC-FUNC-003-WEB-2: Sortowanie wyników według Nutri-Score

**Cel:** Zweryfikować, czy system sortuje wyniki wyszukiwania według Nutri-Score.  

**Warunki wstępne:**
- Strona dostępna pod adresem: https://world.openfoodfacts.org 

**Kroki:**
1. Wyszukaj dowolną kategorię produktów na stronie.
2. Z menu sortowania wybierz opcję "Nutri-Score".

**Oczekiwane wyniki:**
- Wyniki wyszukiwania są posortowane według wartości Nutri-Score w kolejności rosnącej (od A do E).

---

## TC-FUNC-003-WEB-3: Sortowanie wyników według Eco-Score

**Cel:** Zweryfikować, czy system sortuje wyniki wyszukiwania według Eco-Score.  

**Warunki wstępne:**
- Strona dostępna pod adresem: https://world.openfoodfacts.org 

**Kroki:**
1. Wyszukaj dowolną kategorię produktów na stronie.
2. Z menu sortowania wybierz opcję "Eco-Score".

**Oczekiwane wyniki:**
- Wyniki wyszukiwania są posortowane według wartości Eco-Score w kolejności rosnącej (od A do E).

---

## TC-FUNC-004-WEB-1: Weryfikacja dodawania nowych produktów do bazy na stronie internetowej

**Cel:** Sprawdzić, czy użytkownik może dodać nowy produkt, który nie istnieje w bazie danych.

**Warunki wstępne:**
- Strona dostępna pod adresem: https://world.openfoodfacts.org 
- Konto użytkownika z uprawnieniami do edycji.
- W bazie danych brak produktu o podanym kodzie kreskowym.

**Kroki:**
1. Zaloguj się na swoje konto.
2. Rozwiń pasek menu.
3. Przejdź do sekcji "Add a product".
4. Podaj kod lub dodaj zdjęcie kodu kreskowego produktu nieistniejącego w bazie.
5. Wprowadź wszystkie wymagane dane produktu (nazwa, składniki, zdjęcie, kod kreskowy).
6. Kliknij "Save".

**Oczekiwane wyniki:**
- Produkt został poprawnie dodany do bazy.
- Wyświetlany jest komunikat "Added Successfully".
- Nowy produkt jest widoczny w wynikach wyszukiwania.

---

## TC-FUNC-004-WEB-2: Weryfikacja dodawania istniejących produktów do bazy na stronie internetowej

**Cel:** Sprawdzić, czy system blokuje dodanie produktu, który już istnieje w bazie danych.

**Warunki wstępne:**
- Strona dostępna pod adresem: https://world.openfoodfacts.org 
- Konto użytkownika z uprawnieniami do edycji.
- Produkt z tym samym kodem kreskowym istnieje już w bazie danych.

**Kroki:**
1. Zaloguj się na swoje konto.
2. Rozwiń pasek menu.
3. Przejdź do sekcji "Add a product".
4. Podaj kod lub dodaj zdjęcie kodu kreskowego produktu istniejącego w bazie.

**Oczekiwane wyniki:**
- System wyświetla informacje na temat produktu, z możliwością ich edycji.
- Produkt nie zostaje dodany ponownie.

---

## TC-FUNC-004-WEB-3: Weryfikacja dodawania produktów bez kodu kreskowego

**Cel:** Sprawdzić, czy użytkownik może dodać nowy produkt do bazy danych bez kodu kreskowego.

**Warunki wstępne:**
- Strona dostępna pod adresem: https://world.openfoodfacts.org 
- Konto użytkownika z uprawnieniami do edycji.
- Zdjęcie niezawierające kodu kreskowego produktu.

**Kroki:**
1. Zaloguj się na swoje konto.
2. Rozwiń pasek menu.
3. Przejdź do sekcji "Add a product".
4. Dodaj zdjęcie, na którym nie ma żadnego kodu kreskowego.

**Oczekiwane wyniki:**
- Wyświetlany jest komunikat "No barcode found in the image".

---

## TC-FUNC-005-WEB-1: Weryfikacja wyświetlania informacji o alergenach

**Cel:** Zweryfikować, czy system wyświetla informacje o potencjalnych alergenach w produktach.  

**Warunki wstępne:**
- Strona dostępna pod adresem: https://world.openfoodfacts.org 
- Produkt w bazie danych zawiera informacje o alergenach.

**Kroki:**
1. Wyszukaj produkt na stronie internetowej.
2. Przejdź do sekcji "Ingredients".

**Oczekiwane wyniki:**
- Pod listą składników wypisane są alergeny znajdujące się w produkcie.

---

## TC-FUNC-006-WEB-1: Weryfikacja obsługi wielu języków interfejsu

**Cel:** Sprawdzić, czy system obsługuje wiele języków interfejsu użytkownika i w żadnym z nich nie występują błędy.  

**Warunki wstępne:**
- Strona dostępna pod adresem: https://world.openfoodfacts.org/
- System posiada wsparcie dla języka polskiego i angielskiego.

**Kroki:**
1. Będąc na stronie głównej, rozwiń zakładkę "Country".
2. Zmień język interfejsu na wybrany język.
3. Sprawdź, czy wszystkie elementy interfejsu zostały przetłumaczone.
4. Powtórz kroki 1-3 dla obu języków.

**Oczekiwane wyniki:**
- Po zmianie języka, tekst interfejsu jest przetłumaczony na dany język.

---

## TC-FUNC-007-WEB-1: Weryfikacja zgłaszania błędnych lub niekompletnych danych produktu

**Cel:** Zweryfikować, czy użytkownik może zgłaszać i edytować błędne lub niekompletne dane dotyczące produktu.  

**Warunki wstępne:**
- Strona dostępna pod adresem: https://world.openfoodfacts.org/
- Zalogowane konto użytkownika.

**Kroki:**
1. Wyszukaj produkt na stronie, używając "Search a product".
2. Otwórz szczegóły produktu.
3. Kliknij opcję "Edit the page".
4. Wprowadź szczegóły zgłoszenia i je zapisz.

**Oczekiwane wyniki:**
- Zgłoszenie jest wysyłane i widoczny jest komunikat potwierdzający "Changes saved".

---

## TC-FUNC-008-WEB-1: Weryfikacja wyświetlania ocen wartości odżywczych

**Cel:** Sprawdzić, czy system wyświetla oceny wartości odżywczych i wskaźniki zdrowotne dla produktów.  

**Warunki wstępne:**
- Strona dostępna pod adresem: https://world.openfoodfacts.org 
- Produkt zawiera dane wartości odżywczych w bazie danych.

**Kroki:**
1. Wyszukaj produkt na stronie, używając "Search a product".
2. Otwórz szczegóły produktu.

**Oczekiwane wyniki:**
- Wyświetlane są poprawne dane o wartościach odżywczych oraz wskaźniki zdrowotne (np. Nutri-Score).

---

## TC-FUNC-009-WEB-1: Weryfikacja obsługi preferencji dietetycznych użytkownika

**Cel:** Zweryfikować, czy użytkownik może ustawić preferencje dietetyczne, a system automatycznie oznaczy produkty jako zgodne lub niezgodne z tymi preferencjami.  

**Warunki wstępne:**
- Strona dostępna pod adresem: https://world.openfoodfacts.org 
- Zalogowane konto użytkownika.

**Kroki:**
1. Przejdź do ustawień klikając "Edit your preferences".
2. Wybierz preferencje dietetyczne (np. wegańskie, bezglutenowe).
3. Zamknij ustawienia przyciskiem "Close".
4. Wyszukaj produkty w aplikacji.

**Oczekiwane wyniki:**
- Produkty są oznaczone według dopasowania z preferencjami użytkownika.

---

## TC-NFUNC-001-WEB-1: Weryfikacja czasu odpowiedzi systemu

**Cel:** Zweryfikować, czy czas odpowiedzi systemu na zapytania o produkt wynosi mniej niż 2 sekundy w standardowych warunkach testowych.  

**Warunki wstępne:**
- Stabilne połączenie z internetem z ustaloną i zdefiniowaną wartością opóźnienia sieciowego wynoszącą 100 ms.  
- Strona dostępna pod adresem: https://world.openfoodfacts.org 

**Kroki:**
1. Otwórz stronę i wyszukaj produkt.  
2. Zmierz całkowity czas odpowiedzi, wliczając ustaloną wartość opóźnienia sieciowego 100 ms, od momentu wysłania zapytania do wyświetlenia wyników.  

**Oczekiwane wyniki:**
- Wyniki wyszukiwania wyświetlają się w czasie krótszym niż 2 sekundy, uwzględniając ustalone opóźnienie sieciowe.
