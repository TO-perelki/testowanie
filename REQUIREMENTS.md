# Wymagania

Ten dokument przedstawia wymagania funkcjonalne oraz niefunkcjonalne.

---

## Wymagania Funkcjonalne

### REQ-FUNC-001  
**Opis:**  
Program powinien umożliwiać użytkownikom wyszukiwanie produktów według kodu kreskowego.

---

### REQ-FUNC-002  
**Opis:**  
Program musi pozwalać użytkownikom na przeglądanie szczegółowych informacji o składnikach produktów.

---

### REQ-FUNC-003  
**Opis:**  
Program powinien oferować możliwość sortowania wyników wyszukiwania według różnych kryteriów.

---

### REQ-FUNC-004  
**Opis:**  
Program powinien wspierać dodawanie nowych produktów do bazy przez użytkowników.

---

### REQ-FUNC-005  
**Opis:**  
Program powinien wyświetlać informacje o potencjalnych alergenach w produktach.

---

### REQ-FUNC-006  
**Opis:**  
Program musi obsługiwać wiele języków interfejsu użytkownika, takich jak angielski i polski.

---

### REQ-FUNC-007  
**Opis:**  
Program musi umożliwiać użytkownikom zgłaszanie błędnych lub niepełnych danych produktów.

---

### REQ-FUNC-008  
**Opis:**  
Program musi wyświetlać oceny wartości odżywczych oraz wskaźniki zdrowotne, aby pomóc użytkownikom w wyborze zdrowych produktów.

---

### REQ-FUNC-009  
**Opis:**  
Program powinien umożliwiać użytkownikom ustawianie preferencji dietetycznych (np. bezglutenowe, wegańskie, niskosodowe). Po ustawieniu preferencji system automatycznie oznaczy produkty jako zgodne lub niezgodne z preferencjami użytkownika, wyświetlając informację o zgodności dla każdego produktu.

---

## Wymagania Niefunkcjonalne

### REQ-NFUNC-001  
**Opis:**  
System powinien zapewniać czas odpowiedzi krótszy niż 2 sekundy dla zapytań dotyczących wyszukiwania produktów w standardowych warunkach testowych. Standardowe warunki testowe obejmują uwzględnienie stałej i z góry określonej wartości opóźnienia sieciowego wynoszącej 100 ms, aby zapewnić spójne wyniki we wszystkich testach. Łączny czas odpowiedzi powinien być raportowany wraz z opóźnieniem sieciowym dla przejrzystości.

---

### REQ-NFUNC-002  
**Opis:**  
Funkcja skanowania kodów kreskowych powinna działać płynnie, rozpoznając kody w czasie poniżej 1 sekundy z wykorzystaniem standardowych kamer urządzeń mobilnych. Testy będą przeprowadzane w zdefiniowanych warunkach, eliminując zmienność opóźnienia sieciowego poprzez:

- Uruchomienie systemu lokalnie, gdzie opóźnienie sieciowe jest pomijalne.  
- Uwzględnienie stałej i z góry określonej wartości opóźnienia sieciowego wynoszącej 100 ms we wszystkich środowiskach testowych.
