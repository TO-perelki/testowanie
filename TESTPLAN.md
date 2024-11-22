# TESTPLAN.md

## 1. Wprowadzenie

### 1.1 Cel testów
Celem testów jest zapewnienie wysokiej jakości aplikacji Open Food Facts poprzez weryfikację jej funkcjonalności, stabilności oraz wydajności. Testy mają również na celu identyfikację i eliminację potencjalnych błędów przed wdrożeniem nowych funkcji.

### 1.2 Kontekst biznesowy aplikacji
Open Food Facts to otwartoźródłowa baza danych o produktach spożywczych, która pozwala użytkownikom na analizę składników, wartości odżywczych i wpływu produktów na zdrowie. Platforma wspiera zrównoważony rozwój i świadome decyzje konsumentów. Dla społeczności użytkowników kluczowa jest wiarygodność i dostępność danych, dlatego jakość aplikacji ma kluczowe znaczenie.

### 1.3 Zakres testów
#### Funkcjonalności:
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

#### Typy testów:
- Testy funkcjonalne.
- Testy wydajnościowe.
- Testy regresji.

---

## 2. Cele i kryteria testów

### 2.1 Kryteria wejścia
- Kod aplikacji jest stabilny i dostępny w wyznaczonej wersji.
- Dokumentacja wymagań funkcjonalnych i niefunkcjonalnych (REQ-FUNC i REQ-NFUNC) została ukończona.
- Dostępne środowisko testowe oraz dane testowe.
- Zespół testerów oraz ról technicznych został przypisany.

### 2.2 Kryteria wyjścia
- Wykonanie wszystkich zaplanowanych przypadków testowych.
- Brak błędów krytycznych i wysokiego ryzyka.
- Raport końcowy z testów został zatwierdzony przez zespół projektowy.

### 2.3 Kryteria akceptacji wyników testów
- Wszystkie wymagania funkcjonalne (REQ-FUNC-001 do REQ-FUNC-009) zostały zweryfikowane i przetestowane z sukcesem.
- Testy wydajnościowe: czasy odpowiedzi nieprzekraczające 1 sekundy dla 95% żądań.
- Liczba błędów średniego i niskiego priorytetu została oceniona jako akceptowalna i nie wpływa na kluczowe działanie aplikacji.
- Testy regresji: brak regresji w funkcjonalności po wdrożeniu nowych funkcji.

---

## 3. Strategia testowania

### 3.1 Podejście do testowania
- Testy zostaną przeprowadzone w cyklach iteracyjnych, obejmujących różne typy testów.
- Testy funkcjonalne sprawdzą zgodność aplikacji z wymaganiami biznesowymi.
- Testy wydajnościowe ocenią czas odpowiedzi systemu oraz stabilność pod obciążeniem.

### 3.2 Typy testów
- **Testy funkcjonalne:** Weryfikacja działania kluczowych funkcji aplikacji.
- **Testy niefunkcjonalne:** Testy wydajnościowe.
- **Testy regresji:** Sprawdzenie poprawności istniejących funkcji po wprowadzeniu zmian.

### 3.3 Narzędzia i środowisko testowe
- **Narzędzia:**
  - Selenium WebDriver – automatyzacja testów przeglądarkowych.
  - JMeter – testy wydajnościowe.
- **Środowisko:**
  - Serwery testowe z dostępem do najnowszej wersji aplikacji.
  - Dane testowe z bazy Open Food Facts.

---

## 4. Harmonogram i zasoby

### 4.1 Harmonogram testów

- **Listopad (tydzień 2):** Przedstawienie zespołów, ich członków, zadań, zidentyfikowanych ryzyk oraz aplikacji FOSS.  
- **Listopad (tydzień 3):** Przedstawienie specyfikacji wymagań.  
- **Listopad (tydzień 4):** Przedstawienie planów testów.  
- **Grudzień (tydzień 1):** Iteracja 1 przypadków testowych: Przygotowanie wysokopoziomowych przypadków testowych dla każdego obszaru.  
- **Grudzień (tydzień 2):** Iteracja 2 przypadków testowych: Doszczegółowienie (dodanie kroków, danych testowych) oraz przygotowanie puli przypadków dla drugiego zespołu. Losowanie zespołów do testów krzyżowych.  
- **Grudzień (tydzień 3):** Iteracja 1 wyników testów: Przedstawienie wyników testów przeprowadzonych przez inny zespół.  
- **Grudzień (tydzień 4):** Iteracja 2 wyników testów: Przedstawienie wyników własnych testów z ostatniego tygodnia.  
- **Styczeń (tydzień 1):** Iteracja 3 wyników testów: Przedstawienie wyników testów z ostatniego tygodnia.  
- **Styczeń (tydzień 2):** Iteracja 4 wyników testów: Przedstawienie wyników testów z ostatniego tygodnia.  
- **Styczeń (tydzień 3):** Raporty z testów: Prezentacja wyników i jednostronicowe podsumowanie.  
- **Styczeń (tydzień 4):** Rezerwa czasowa: Czas na ewentualne poprawki i uzupełnienia.  


### 4.2 Role i odpowiedzialności
| Rola                    | Osoba           | Zakres odpowiedzialności                                        |
|-------------------------|-----------------|----------------------------------------------------------------|
| Kierownik testów        | Kacper i Oliwia | Planowanie i zarządzanie testami.                              |
| Tester funkcjonalny     | Kacper i Oliwia | Testy zgodności z wymaganiami.                                 |
| Tester wydajnościowy    | Kacper i Oliwia | Analiza wydajności aplikacji.                                  |
| Tester regresji       | Kacper i Oliwia | Weryfikacja, czy zmiany w systemie nie wpłynęły negatywnie.   |

---

## 5. Zarządzanie ryzykiem

### 5.1 Potencjalne ryzyka i ich wpływ
- **Brak dostępu do środowiska testowego:** Opóźnienia w realizacji testów.
- **Niekompletne wymagania:** Niewłaściwe przygotowanie przypadków testowych.
- **Błędy krytyczne wykryte zbyt późno:** Konieczność opóźnienia wdrożenia.
- **Niekompletne dane testowe:** Mogą wpływać na wyniki.
- **Niespodziewane zmiany w kodzie:** Mogą wymagać dodatkowych testów.
- **Brak doświadczenia w testowaniu aplikacji open-source:** Utrudnienie skutecznego testowania.
- **Niedostateczne zasoby czasowe:** Brak możliwości przetestowania wszystkich funkcji.

### 5.2 Plany łagodzenia ryzyka
- Regularna komunikacja z zespołem deweloperskim.
- Weryfikacja wymagań przed rozpoczęciem testów.
- Przygotowanie kopii zapasowych danych testowych.
- Bliska współpraca z zespołem deweloperskim, aby na bieżąco wprowadzać poprawki.
- Zapoznanie się z zasadami i etykietą pracy w projektach open-source.
- Ustalanie priorytetów testów i realistyczne planowanie działań.

---

## 6. Metryki i raportowanie

### 6.1 Kluczowe wskaźniki jakości
- Procent wykonanych przypadków testowych.
- Liczba wykrytych błędów krytycznych.
- Czas naprawy błędów.
- Średni czas reakcji na zapytanie (wydajność).

### 6.2 Sposób raportowania wyników testów
- Raporty postępu testów:
  - Podsumowanie wykonanych testów, wykrytych błędów oraz postępów w realizacji harmonogramu.
  - Liczba przypadków testowych wykonanych i zakończonych sukcesem.
  - Liczba wykrytych błędów.
  - Status błędów (nowe, naprawione, ponownie otwarte).
- Raport końcowy z podsumowaniem wszystkich wyników testów, w tym:
  - Liczba wykrytych błędów według priorytetów.
  - Wyniki testów wydajnościowych.
  - Ocena zgodności z kryteriami akceptacji.

