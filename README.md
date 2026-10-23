# Półmaraton Wrocławski 2024

Aplikacja w Streamlit do przeglądania wyników Półmaratonu Wrocławskiego 2024.

## Cel projektu

Szybki podgląd wyników zawodów bez otwierania arkusza z danymi: kto wygrał, skąd byli
zawodnicy, jak rozkładały się czasy na mecie i które parametry biegu są ze sobą powiązane.

## Co potrafi aplikacja

- filtrowanie zawodników po imieniu, kraju, kategorii wiekowej i płci,
- liczba zawodników, mężczyzn i kobiet dla wybranych filtrów,
- top 5 zawodników i 10 losowych wyników,
- wykres pochodzenia zawodników (kraje),
- histogram czasu na mecie,
- macierz korelacji dla danych liczbowych (czasy, tempo, miejsca).

## Dane

Plik `halfmarathon_wroclaw_2024__final.csv` (separator `;`) – oficjalne wyniki zawodów:
miejsce, numer startowy, kraj, kategoria wiekowa, rocznik, międzyczasy i tempo na 5, 10, 15
i 20 km oraz czas końcowy.

## Uruchomienie

```
pip install -r requirements.txt
streamlit run app.py
```

## Plan rozwoju

- przewidywanie czasu na mecie na podstawie wieku, płci i czasu na 5 km,
- porównanie z wynikami z 2023 roku,
- wdrożenie aplikacji w chmurze.
