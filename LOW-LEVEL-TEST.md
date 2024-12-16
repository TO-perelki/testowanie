# Szczegółowe Przypadki Testowe

## TC-FUNC-001: Weryfikacja wyszukiwania produktów po kodzie kreskowym
**Cel:** Zweryfikować, czy użytkownik może skutecznie wyszukać produkty za pomocą kodu kreskowego.  
**Warunki wstępne:**
- Urządzenie z aplikacją zainstalowaną i zalogowanym użytkownikiem.
- Produkt z widocznym kodem kreskowym.

**Kroki:**
1. Uruchom aplikację na urządzeniu mobilnym.
2. Przejdź do sekcji "Wyszukiwanie produktów".
3. Wybierz opcję "Skanuj kod kreskowy".
4. Nakieruj kamerę na kod kreskowy produktu.
5. Poczekaj na automatyczne rozpoznanie kodu przez aplikację.

**Oczekiwane wyniki:**
- Kod kreskowy zostaje poprawnie zeskanowany.
- Wyświetlają się szczegółowe informacje o produkcie powiązanym z kodem kreskowym.

---

## TC-FUNC-002: Weryfikacja wyświetlania szczegółowych informacji o składnikach produktu
**Cel:** Sprawdzić, czy użytkownik ma dostęp do szczegółowych informacji o składnikach każdego produktu.  
**Warunki wstępne:**
- Produkt istnieje w bazie danych.

**Kroki:**
1. Otwórz aplikację i przejdź do wyszukiwania produktu.
2. Wprowadź nazwę produktu w polu wyszukiwania i naciśnij "Szukaj".
3. Wybierz produkt z listy wyników wyszukiwania.

**Oczekiwane wyniki:**
- Wyświetlane są szczegółowe informacje o składnikach produktu, w tym ich ilości, pochodzenie i wartości odżywcze.

---

## TC-FUNC-003.1: Sortowanie wyników według najczęściej skanowanych produktów
**Cel:** Zweryfikować, czy system sortuje wyniki wyszukiwania według najczęściej skanowanych produktów.  
**Warunki wstępne:**
- Strona dostępna pod adresem: https://world.openfoodfacts.org/

**Kroki:**
1. Wyszukaj dowolną kategorię produktów w aplikacji.
2. Z menu sortowania wybierz opcję "Najczęściej skanowane".

**Oczekiwane wyniki:**
- Wyniki wyszukiwania są posortowane według liczby skanowań w kolejności malejącej.

---

## TC-FUNC-003.2: Sortowanie wyników według Nutri-Score
**Cel:** Zweryfikować, czy system sortuje wyniki wyszukiwania według Nutri-Score.  
**Warunki wstępne:**
- Strona dostępna pod adresem: https://world.openfoodfacts.org/

**Kroki:**
1. Wyszukaj dowolną kategorię produktów w aplikacji.
2. Z menu sortowania wybierz opcję "Nutri-Score".

**Oczekiwane wyniki:**
- Wyniki wyszukiwania są posortowane według wartości Nutri-Score w kolejności rosnącej (od A do E).

---

## TC-FUNC-003.3: Sortowanie wyników według Eco-Score
**Cel:** Zweryfikować, czy system sortuje wyniki wyszukiwania według Eco-Score.  
**Warunki wstępne:**
- Strona dostępna pod adresem: https://world.openfoodfacts.org/

**Kroki:**
1. Wyszukaj dowolną kategorię produktów w aplikacji.
2. Z menu sortowania wybierz opcję "Eco-Score".

**Oczekiwane wyniki:**
- Wyniki wyszukiwania są posortowane według wartości Eco-Score w kolejności rosnącej (od A do E).

---

## TC-FUNC-004.1: Weryfikacja dodawania nowych produktów do bazy na stronie internetowej
**Cel:** Sprawdzić, czy użytkownik może dodać nowy produkt, który nie istnieje w bazie danych.

**Warunki wstępne:**
- Konto użytkownika z uprawnieniami do edycji.
- W bazie danych brak produktu o podanym kodzie kreskowym.

**Kroki:**
1. Zaloguj się na swoje konto.
2. Rozwiń pasek menu.
3. Przejdź do sekcji "Add a product".
4. Podaj kod, lub dodaj zdjęcie kodu kreskowego produktu nieistniejącego w bazie.
5. Wprowadź wszystkie wymagane dane produktu (nazwa, składniki, zdjęcie, kod kreskowy).
6. Kliknij "Save".

**Oczekiwane wyniki:**
- Produkt został poprawnie dodany do bazy.
- Wyświetlany jest komunikat "Added Successfully".
- Nowy produkt jest widoczny w wynikach wyszukiwania.

---

## TC-FUNC-004.2: Weryfikacja dodawania istniejących produktów do bazy na stronie internetowej
**Cel:** Sprawdzić, czy system blokuje dodanie produktu, który już istnieje w bazie danych.

**Warunki wstępne:**
- Konto użytkownika z uprawnieniami do edycji.
- Produkt z tym samym kodem kreskowym istnieje już w bazie danych.

**Kroki:**
1. Zaloguj się na swoje konto.
2. Rozwiń pasek menu.
3. Przejdź do sekcji "Add a product".
4. Podaj kod, lub dodaj zdjęcie kodu kreskowego produktu istniejącego w bazie.

**Oczekiwane wyniki:**
- System wyświetla informacje na temat produktu, z możliwością ich edycji.
- Produkt nie zostaje dodany ponownie.

---

## TC-FUNC-004.3: Weryfikacja dodawania nieistniejących produktów do bazy w aplikacji mobilnej
**Cel:** Sprawdzić, czy użytkownik może dodać nowy produkt, który nie istnieje w bazie danych.

**Warunki wstępne:**
- Konto użytkownika z uprawnieniami do edycji.
- W bazie danych brak produktu o podanym kodzie kreskowym.

**Kroki:**
1. Zaloguj się na swoje konto.
2. Zeskanuj w aplikacji kod kreskowy produktu, który nie istnieje w bazie.
3. Uzupełnij podstawowe informacje tj. zdjęcie, nazwa produktu, nazwa marki, ilość i waga.
4. Kliknij przycisk "Zapisz".

**Oczekiwane wyniki:**
- Wyświetla się komunikat o poprawnym dodaniu produktu.
- Produkt został dodany do bazy danych.

---

## TC-FUNC-004.4: Weryfikacja dodawania nowych produktów do bazy na stronie internetowej
**Cel:** Sprawdzić, czy użytkownik może dodać nowy produkt do bazy danych.

**Warunki wstępne:**
- Konto użytkownika z uprawnieniami do edycji.
- Zdjęcie niezawierające kodu kreskowego produktu.

**Kroki:**
1. Zaloguj się na swoje konto.
2. Rozwiń pasek menu.
3. Przejdź do sekcji "Add a product".
4. Dodaj zdjęcie, na którym brak kodu kreskowego.

**Oczekiwane wyniki:**
- Wyświetlany jest komunikat "No barcode found in the image.".

---

## TC-FUNC-005: Weryfikacja wyświetlania informacji o alergenach
**Cel:** Zweryfikować, czy system wyświetla informacje o potencjalnych alergenach w produktach.  
**Warunki wstępne:**
- Produkt w bazie danych zawiera informacje o alergenach.

**Kroki:**
1. Wyszukaj produkt w aplikacji.
2. Przejdź do sekcji "Szczegóły produktu".

**Oczekiwane wyniki:**
- Informacje o alergenach sąwidoczne w sekcji szczegółów produktu.

---

## TC-FUNC-006: Weryfikacja obsługi wielu języków interfejsu
**Cel:** Sprawdzić, czy system obsługuje wiele języków interfejsu użytkownika i w żadnym z nich nie występują błędy.  
**Warunki wstępne:**
- System posiada wsparcie dla języka polskiego i angielskiego.

**Kroki:**
1. Przejdź do ustawień aplikacji.
2. Zmień język interfejsu na wybrany język.
3. Sprawdź, czy wszystkie elementy interfejsu zostały przetłumaczone.
4. Powtórz kroki 1-3 dla obu języków.

**Oczekiwane wyniki:**
- Wszystkie elementy interfejsu są poprawnie przetłumaczone bez błędów.

---

## TC-FUNC-007: Weryfikacja zgłaszania błędnych lub niekompletnych danych produktu
**Cel:** Zweryfikować, czy użytkownik może zgłaszać błędne lub niekompletne dane dotyczące produktu.  
**Warunki wstępne:**
- Zalogowane konto użytkownika.

**Kroki:**
1. Wyszukaj produkt w aplikacji.
2. Otwórz szczegóły produktu.
3. Kliknij opcję "Edit the page".
4. Wprowadź szczegóły zgłoszenia i je zapisz.

**Oczekiwane wyniki:**
- Zgłoszenie jest wysyłane i widoczny jest komunikat potwierdzający "Changes saved.".

---

## TC-FUNC-008: Weryfikacja wyświetlania ocen wartości odżywczych
**Cel:** Sprawdzić, czy system wyświetla oceny wartości odżywczych i wskaźniki zdrowotne dla produktów.  
**Warunki wstępne:**
- Produkt zawiera dane wartości odżywczych w bazie danych.

**Kroki:**
1. Wyszukaj produkt w aplikacji.
2. Przejdź do sekcji "Wartości odżywcze" w szczegółach produktu.

**Oczekiwane wyniki:**
- Wyświetlane są poprawne dane o wartościach odżywczych oraz wskaźniki zdrowotne (np. Nutri-Score).

---

## TC-FUNC-009: Weryfikacja obsługi preferencji dietetycznych użytkownika
**Cel:** Zweryfikować, czy użytkownik może ustawić preferencje dietetyczne, a system automatycznie oznaczy produkty jako zgodne lub niezgodne z tymi preferencjami.  
**Warunki wstępne:**
- Konto użytkownika.

**Kroki:**
1. Przejdź do ustawień klikając "Edit your preferences".
2. Wybierz preferencje dietetyczne (np. wegańskie, bezglutenowe).
3. Zamknij ustawienia przyciskiem close.
4. Wyszukaj produkty w aplikacji.

**Oczekiwane wyniki:**
- Produkty są oznaczone jako zgodne lub niezgodne z preferencjami użytkownika.

---

## TC-NFUNC-001: Weryfikacja czasu odpowiedzi systemu
**Cel:** Sprawdzić, czy czas odpowiedzi systemu dla zapytania o produkt wynosi mniej niż 2 sekundy.  
**Warunki wstępne:**
- Stabilne połączenie z internetem.

**Kroki:**
1. Wyszukaj produkt w aplikacji.
2. Zmierz czas od momentu wysłania zapytania do wyświetlenia wyników.

**Oczekiwane wyniki:**
- Wyniki wyszukiwania wyświetlają się w czasie krótszym niż 2 sekundy.

---

## TC-NFUNC-002: Weryfikacja płynności działania funkcji skanowania kodów kreskowych
**Cel:** Sprawdzić, czy funkcja skanowania kodów kreskowych działa płynnie i rozpoznaje kody w czasie krótszym niż 1 sekunda przy użyciu standardowych kamer urządzeń mobilnych.  
**Warunki wstępne:**
- Urządzenie z funkcjonalną kamerą.

**Kroki:**
1. Otwórz aplikację i wybierz funkcję skanowania kodów kreskowych.
2. Nakieruj kamerę na kod kreskowy.
3. Zmierz czas od momentu nakierowania kamery do momentu rozpoznania kodu.

**Oczekiwane wyniki:**
- Kod kreskowy jest rozpoznawany w czasie krótszym niż 1 sekunda.
