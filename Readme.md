# Lupus Agent - Operacyjna Automatyzacja Monitoringu Kosztów

## 📋 O projekcie
Lupus Agent to autorski skrypt napisany w języku Python, stworzony w celu automatyzacji zarządzania finansami Narzędzie rozwiązuje problem rozproszonych faktur od wielu dostawców mediów i usług, monitorując skrzynkę e-mail w czasie rzeczywistym.

Jest to projekt łączący umiejętności programistyczne z analitycznym podejściem do optymalizacji procesów oraz zarządzania budżetem i terminami płatności.

## 🚀 Funkcjonalności
- **Automatyczny Skaner:** Skrypt przeszukuje nieprzeczytane wiadomości e-mail pod kątem zdefiniowanej listy dostawców (np. nju, PGE, PGNiG, E.ON).
- **Powiadomienia Telegram:** Natychmiastowe wysyłanie kluczowych informacji o fakturach bezpośrednio na telefon właściciela floty.
- **Bezpieczeństwo (Data Privacy):** Pełna separacja danych wrażliwych (hasła, tokeny, adresy email) od kodu źródłowego przy użyciu zmiennych środowiskowych (Environment Variables).
- **Obsługa błędów:** Wbudowane mechanizmy logowania błędów i bezpiecznego zamykania sesji IMAP.

## 🛠️ Technologie
- **Python 3.x**
- **IMAPLib & Email:** Integracja z serwerem poczty Gmail.
- **PyTelegramBotAPI:** Komunikacja z botem Telegram.
- **Linux Bash:** Zarządzanie konfiguracją środowiska na serwerze (PythonAnywhere).

## 📈 Zastosowanie w Analityce Danych
Projekt ten stanowi fundament pod system zbierania danych kosztowych (Data Acquisition). Pozyskane w ten sposób informacje mogą być docelowo agregowane w bazie danych SQL, a następnie wizualizowane w Tableau/PowerBI w celu analizy rentowności każdego pojazdu we flocie.

## ⚙️ Konfiguracja
Skrypt wymaga ustawienia następujących zmiennych środowiskowych:
- `LUPUS_EMAIL` - adres monitorowanej skrzynki.
- `LUPUS_PwD` - hasło aplikacji Gmail.
- `TELEGRAM_TOKEN` - token bota z BotFather.
- `TELEGRAM_CHAT_ID` - identyfikator czatu użytkownika.

---
*Projekt zrealizowany przez Andrzeja w ramach budowy portfolio Junior Data Analyst.*