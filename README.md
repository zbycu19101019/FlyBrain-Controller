# FlyBrain Controller 2.0.5

Lokalny prototyp sterownika Android przez ADB, z analizą obrazu, OCR, planowaniem MCTS i syntetyczną siecią 1000 neuronów LIF. Aplikacja dla Windows x64.

## Uruchomienie

- Instalator: uruchom `FlyBrainController-Setup-2.0.5-x64.exe`.
- Wersja przenośna: rozpakuj cały ZIP i uruchom `START.cmd`. Nie przenoś samego EXE bez katalogu `_internal`.
- Kod źródłowy: zainstaluj Python 3.12, uruchom `Source/SETUP.cmd`, następnie `Source/START.cmd`.

Telefon wymaga ADB, włączonego debugowania i zatwierdzenia komputera. Narzędzia Android platform-tools należy pobrać ze strony producenta. Kalibrację wykonuje każdy użytkownik dla własnego urządzenia i gry.

## Dane

Paczka nie zawiera profilu telefonu, danych logowania, numeru urządzenia, prywatnych zrzutów ekranu, logów ani próbek OCR pochodzących z telefonu. Model OCR zawiera wyłącznie syntetyczne cyfry z fontów. Modele offline zostały wytrenowane na symulatorze, nie na prywatnej rozgrywce.

Dane powstające podczas używania aplikacji są zapisywane lokalnie w `%LOCALAPPDATA%/FlyBrainController/Data`. Aplikacja nie wysyła ich na GitHub. Wersja przenośna również używa tego katalogu. Aktualizacja zachowuje istniejące dane lokalne.

## Ograniczenia

To prototyp, a nie gwarancja automatycznego przejścia gry. Reguły silnika wymagają weryfikacji. Rozpoznawanie cyfr syntetycznych nie jest pomiarem skuteczności na telefonie. Nierozpoznane reklamy i niepotwierdzone gesty mogą zatrzymać automat. Większa sieć nie gwarantuje lepszego wyniku.

Biblioteki i ich licencje znajdują się w `LICENSES` w dystrybucji Windows.
