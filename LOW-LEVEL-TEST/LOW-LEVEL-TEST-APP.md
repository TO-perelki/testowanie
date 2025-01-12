# Przypadki Testowe dla Aplikacji

## TC-FUNC-001-APP-1 : Weryfikacja wyszukiwania produktów po kodzie kreskowym
**Cel:** Zweryfikować, czy użytkownik może skutecznie wyszukać produkty za pomocą kodu kreskowego.  
**Warunki wstępne:**
- Urządzenie z aplikacją zainstalowaną i zalogowanym użytkownikiem.
- Produkt, który znajduje się w bazie, z widocznym kodem kreskowym.

**Kroki:**
1. Uruchom aplikację na urządzeniu mobilnym.
2. Wejdź w zakładkę "Skanuj".
3. Nakieruj kamerę na kod kreskowy produktu.
4. Poczekaj na automatyczne rozpoznanie kodu przez aplikację.

**Oczekiwane wyniki:**
- Kod kreskowy zostaje poprawnie zeskanowany.
- Wyświetlają się szczegółowe informacje o produkcie powiązanym z kodem kreskowym.

---

## TC-FUNC-001-APP-2 : Weryfikacja wyszukiwania produktów po kodzie kreskowym (produktów nieistniejących w bazie)
**Cel:** Zweryfikować, czy użytkownik może skutecznie wyszukać produkty za pomocą kodu kreskowego, których nie ma w bazie.  
**Warunki wstępne:**
- Urządzenie z aplikacją zainstalowaną i zalogowanym użytkownikiem.
- Produkt, który nie znajduje się w bazie, z widocznym kodem kreskowym.

**Kroki:**
1. Uruchom aplikację na urządzeniu mobilnym.
2. Wejdź w zakładkę "Skanuj".
3. Nakieruj kamerę na kod kreskowy produktu.
4. Poczekaj na automatyczne rozpoznanie kodu przez aplikację.

**Oczekiwane wyniki:**
- Kod kreskowy zostaje poprawnie zeskanowany.
- Wyświetla się komunikat "Nieznany produkt" z możliwością dodania go do bazy.

---

## TC-FUNC-002-APP-1: Weryfikacja wyświetlania szczegółowych informacji o składnikach produktu
**Cel:** Sprawdzić, czy użytkownik ma dostęp do szczegółowych informacji o składnikach każdego produktu.  
**Warunki wstępne:**
- Urządzenie z aplikacją zainstalowaną i zalogowanym użytkownikiem.
- Produkt istnieje w bazie danych.

**Kroki:**
1. Otwórz aplikację i przejdź do zakładki "Skanuj".
2. Wprowadź nazwę produktu w polu wyszukiwania i naciśnij symbol lupy, wybierz produkt z listy wyników wyszukiwania lub zeskanuj kod kreskowy produktu.
3. Kliknij "Kliknij, aby wyświetlić więcej informacji...".

**Oczekiwane wyniki:**
- Wyświetlane są szczegółowe informacje o składnikach produktu, w tym ich ilości, pochodzenie i wartości odżywcze.

---

## TC-FUNC-004-APP-1: Weryfikacja dodawania nieistniejących produktów do bazy w aplikacji mobilnej
**Cel:** Sprawdzić, czy użytkownik może dodać nowy produkt, który nie istnieje w bazie danych.

**Warunki wstępne:**
- Urządzenie z aplikacją zainstalowaną i zalogowanym użytkownikiem.
- W bazie danych brak produktu o podanym kodzie kreskowym.

**Kroki:**
1. Zaloguj się na swoje konto.
2. Zeskanuj w aplikacji kod kreskowy produktu, który nie istnieje w bazie.
3. Wybierz "Dodaj produkt".
4. Uzupełnij podstawowe informacje tj. zdjęcie produktu z przodu, zdjęcie listy składników, zdjęcie tabeli wartości odżywczych, zdjęcie informacji dotyczących recyklingu.
5. Naciśnij "Następne" i uzupełnij kategorię produktu, wartości odżywcze.
6. Kliknij przycisk "Zakończ".

**Oczekiwane wyniki:**
- Wyświetla się komunikat o poprawnym dodaniu produktu.
- Produkt został dodany do bazy danych.

---

## TC-FUNC-005-APP-1 : Weryfikacja wyświetlania informacji o alergenach
**Cel:** Zweryfikować, czy system wyświetla informacje o potencjalnych alergenach w produktach.  
**Warunki wstępne:**
- Urządzenie z aplikacją zainstalowaną i zalogowanym użytkownikiem.
- Produkt w bazie danych zawiera informacje o alergenach.

**Kroki:**
1. Wyszukaj produkt w aplikacji.
2. Przejdź do sekcji "Szczegóły produktu".
3. W tabeli "Zdrowie" kliknij w zakładkę "Składniki".

**Oczekiwane wyniki:**
- Pod listą składników wypisane są alergeny znajdujące się w produkcie.

---

## TC-FUNC-006-APP-1: Weryfikacja obsługi wielu języków interfejsu
**Cel:** Sprawdzić, czy system obsługuje wiele języków interfejsu użytkownika.

**Warunki wstępne:**
- System posiada wsparcie dla języka polskiego i angielskiego.
- Urządzenie z aplikacją zainstalowaną i zalogowanym użytkownikiem.

**Kroki:**
1. Uruchom aplikację.
2. Przejdź do zakładki "Profil".
3. Przejdź do zakładki "Ustawienia".
4. Wybierz język aplikacji.
5. Sprawdź, czy elementy interfejsu zostały przetłumaczone.
6. Powtórz kroki 1-5 dla obu języków.

**Oczekiwane wyniki:**
- Po zmianie języka, tekst interfejsu jest przetłumaczony na dany język.

---

## TC-FUNC-007-APP-1: Weryfikacja edytowania błędnych lub niekompletnych danych produktu
**Cel:** Zweryfikować, czy użytkownik może edytować błędne lub niekompletne dane dotyczące produktu.  
**Warunki wstępne:**
- Urządzenie z aplikacją zainstalowaną i zalogowanym użytkownikiem.
- Produkt znajdujący się w bazie danych.

**Kroki:**
1. Wyszukaj produkt w aplikacji.
2. Otwórz szczegóły produktu.
3. Kliknij opcję "Edytuj".
4. Wprowadź zmiany w błędnych lub niekompletnych danych i je zapisz.

**Oczekiwane wyniki:**
- Dane zostały zmienione, co zostaje potwierdzone komunikatem.

---

## TC-FUNC-008-APP-1: Weryfikacja wyświetlania ocen wartości odżywczych
**Cel:** Sprawdzić, czy system wyświetla oceny wartości odżywczych i wskaźniki zdrowotne dla produktów.  
**Warunki wstępne:**
- Urządzenie z aplikacją zainstalowaną i zalogowanym użytkownikiem.
- Produkt zawiera dane wartości odżywczych w bazie danych.

**Kroki:**
1. Wyszukaj produkt w aplikacji.
2. Przejdź do sekcji "Szczegóły produktu".

**Oczekiwane wyniki:**
- Wyświetlane są poprawne dane o wartościach odżywczych oraz wskaźniki zdrowotne (np. Nutri-Score, jakość odżywcza, zawartość cukrów, tłuszczów).

---

## TC-FUNC-009-APP-1: Weryfikacja obsługi preferencji dietetycznych użytkownika
**Cel:** Zweryfikować, czy użytkownik może ustawić preferencje dietetyczne, a system automatycznie oznaczy produkty jako zgodne lub niezgodne z tymi preferencjami.  
**Warunki wstępne:**
- Urządzenie z aplikacją zainstalowaną i zalogowanym użytkownikiem.

**Kroki:**
1. Przejdź do zakładki "Profil".
2. Przejdź do zakładki "Preferencje żywieniowe".
3. Wybierz własne preferencje dietetyczne.
4. Wyszukaj produkty w aplikacji.

**Oczekiwane wyniki:**
- Produkty są oznaczone według dopasowania z preferencjami użytkownika.

---

## TC-NFUNC-002-APP-1: Weryfikacja płynności działania funkcji skanowania kodów kreskowych
**Cel:** Zweryfikować, czy funkcja skanowania kodów kreskowych działa płynnie i rozpoznaje kody w czasie krótszym niż 1 sekunda przy użyciu standardowych kamer urządzeń mobilnych, w standardowych warunkach testowych.  

**Warunki wstępne:**  
- Urządzenie z aplikacją zainstalowaną i zalogowanym użytkownikiem oraz funkcjonalną kamerą.
- Testy przeprowadzane w warunkach z wyeliminowaną zmiennością opóźnień sieciowych, tj.:  
  - System uruchomiony lokalnie, gdzie opóźnienia sieciowe są znikome, lub  
  - W środowisku testowym z ustaloną wartością opóźnienia sieciowego wynoszącą 100 ms.  

**Kroki:**  
1. Otwórz aplikację.  
2. Nakieruj kamerę urządzenia na kod kreskowy.  
3. Zmierz czas od momentu nakierowania kamery na kod do momentu jego rozpoznania.  

**Oczekiwane wyniki:**  
- Kod kreskowy jest rozpoznawany w czasie krótszym niż 1 sekunda.
