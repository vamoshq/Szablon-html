# Podgląd Artykułów - System Wizualizacji

## Opis projektu
System składa się z dwóch szablonów HTML służących do podglądu artykułów w formacie Markdown. Projekt zawiera wersję z edytorem do szybkiego podglądu oraz wersję do wyświetlania artykułu z pliku tekstowego.

## Struktura projektu
```
├── szablon.html     # Interaktywny szablon z edytorem
├── podglad.html     # Szablon wczytujący artykuł z pliku
├── zadanie.txt      # Plik z treścią artykułu (wymagany dla podglad.html)
└── README.md        # Dokumentacja projektu
```

## Funkcjonalności

### szablon.html
- Interaktywny edytor tekstu
- Podgląd na żywo podczas wpisywania
- Obsługa formatowania Markdown
- Responsywny design
- Stylowanie dla różnych elementów tekstu (nagłówki, cytaty, kod, etc.)

### podglad.html
- Automatyczne wczytywanie artykułu z pliku zadanie.txt
- Obsługa formatowania Markdown
- Responsywny design
- Obsługa błędów wczytywania pliku


## Jak używać

### Szablon z edytorem (szablon.html)
1. Otwórz plik `szablon.html` w przeglądarce
2. Wklej lub wpisz tekst w formacie Markdown w pole tekstowe
3. Podgląd automatycznie się zaktualizuje

### Podgląd z pliku (podglad.html)
1. Umieść treść artykułu w pliku `zadanie.txt` w formacie Markdown
2. Umieść plik `zadanie.txt` w tym samym folderze co `podglad.html`
3. Otwórz `podglad.html` w przeglądarce

## Obsługiwane elementy Markdown
- Nagłówki (# ## ### itd.)
- Pogrubienie (**tekst**)
- Kursywa (*tekst*)
- Linki [tekst](url)
- Listy (uporządkowane i nieuporządkowane)
- Cytaty (> tekst)
- Kod (`kod` oraz bloki kodu)
- Obrazy ![alt](url)

## Uwagi
- Pliki są całkowicie samodzielne (wszystkie style i skrypty są zawarte w jednym pliku)
- Biblioteka Marked.js jest ładowana z CDN
- System nie wymaga instalacji dodatkowego oprogramowania
- W przypadku problemów z wczytaniem pliku zadanie.txt, sprawdź czy:
  - Plik istnieje w odpowiednim folderze
  - Nazwa pliku jest poprawna (zadanie.txt)
  - Plik ma odpowiednie uprawnienia do odczytu