# Raport z testów aplikacji OpenFoodFacts

## 1. Wprowadzenie

### 1.1. Zakres testów

- Wyszukiwanie produktów według kodu kreskowego (REQ-FUNC-001).
- Przeglądanie szczegółowych informacji o składnikach produktów (REQ-FUNC-002).
- Sortowanie wyników wyszukiwania według różnych kryteriów (REQ-FUNC-003).
- Dodawanie nowych produktów przez użytkowników (REQ-FUNC-004).
- Wyświetlanie informacji o alergenach i preferencjach dietetycznych (REQ-FUNC-005, REQ-FUNC-009).
- Obsługa wielu języków interfejsu (REQ-FUNC-006).
- Zgłaszanie błędów w danych (REQ-FUNC-007).
- Oceny zdrowotne produktów (REQ-FUNC-008).
- Czas odpowiedzi na zapytania poniżej 2 sekund (REQ-NFUNC-001).
- Rozpoznanie kodu w czasie krótszym niż 1 sekunda (REQ-NFUNC-002).

### 1.2. Zespół testowy

- **Oliwia Cyganek** - pisanie przypadków testowych, przeprowadzanie testów, przygotowywanie dokumentacji.
- **Kacper Dominiec** - pisanie przypadków testowych, przeprowadzanie testów, przygotowywanie dokumentacji.

## 2. Statystyki testów

| Platforma | Testy wykonane/zaliczone | Znalezione defekty |
| --------- | ------------------------ | ------------------ |
| APP       | 10/9                     | 1                  |
| WEB       | 13/10                     | 8                  |

## 3. Zaraportowane defekty

- [Invalid Address Error When Accessing the Last Page of Additive Listings](https://github.com/openfoodfacts/openfoodfacts-server/issues/11282)
- [Inappropriate Error Handling When Adding Images Without a Barcode](https://github.com/openfoodfacts/openfoodfacts-server/issues/11253)
- [Barcode Overflow in Search Results for Logged-in Users](https://github.com/openfoodfacts/openfoodfacts-server/issues/11252)
- [Error on Eco-Score A+ page: MongoDB Database Error](https://github.com/openfoodfacts/openfoodfacts-server/issues/11033)
- [Results Per Page Setting Fails to Display More Than 100 Items](https://github.com/openfoodfacts/openfoodfacts-server/issues/11261)
- [Empty Pages in Environmental Score Range 440–481](https://github.com/openfoodfacts/openfoodfacts-server/issues/11260)
- [Page Numbers Are Merging Together, Making Them Unreadable](https://github.com/openfoodfacts/openfoodfacts-server/issues/11257)

## 4. Podsumowanie

Przeprowadzone testy aplikacji OpenFoodFacts pozwoliły na pełne pokrycie wszystkich wymagań funkcjonalnych i niefunkcjonalnych. Dzięki starannie opracowanemu planowi testów udało się uniknąć potencjalnych ryzyk, co pozwoliło na skuteczne przeprowadzenie testów oraz wykrycie kluczowych problemów. Zidentyfikowane defekty dotyczą głównie aplikacji webowej, w tym problemów związanych z wyświetlaniem wyników lub niedziałający UI. Zaleca się dalsze testy regresyjne po wdrożeniu poprawek.

Repozytorium aplikacji dostępne jest pod adresem: [GitHub - OpenFoodFacts](https://github.com/openfoodfacts/)

