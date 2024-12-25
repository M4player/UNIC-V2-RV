# UNIC V2 RV

**UNIC V2 RV** to narzędzie do usuwania plików tymczasowych, plików cache oraz logów z platform gier takich jak Epic Games oraz Steam. Program umożliwia także integrację z Discord, wysyłając powiadomienia o zakończeniu procesu czyszczenia.

## Funkcje

- **Usuwanie plików tymczasowych:** Program skanuje system w poszukiwaniu plików tymczasowych, które mogą zajmować cenne miejsce na dysku.
- **Usuwanie plików cache:** Usuwa pliki cache z aplikacji takich jak Epic Games oraz Steam, co pomaga zwolnić miejsce oraz poprawić wydajność.
- **Usuwanie logów:** Program usuwa logi generowane przez Epic Games i Steam, które mogą zawierać zbędne dane.
- **Webhook Discord:** Po zakończeniu procesu czyszczenia, UNIC V2 RV może wysłać powiadomienie na wskazany kanał Discord, informując użytkownika o ukończeniu zadania.

## Instalacja

1. Pobierz plik wykonywalny **UNIC V2 RV** z [linku do pobrania].
2. Uruchom program. Program nie wymaga instalacji.

## Jak używać

1. Uruchom program **UNIC V2 RV**.
2. Wybierz opcje, które chcesz, aby program wykonał:
   - Usuwanie plików tymczasowych
   - Usuwanie plików cache
   - Usuwanie logów z Epic Games i Steam
3. Opcjonalnie, skonfiguruj webhook Discord w pliku konfiguracyjnym.
4. Kliknij przycisk "Rozpocznij czyszczenie", aby rozpocząć proces.
5. Program przeprowadzi czyszczenie i powiadomi cię o zakończeniu.

## Webhook Discord

Aby skonfigurować webhook Discord:

1. Zaloguj się na swoje konto Discord.
2. Wejdź na kanał, na który chcesz wysyłać powiadomienia.
3. Kliknij prawym przyciskiem myszy na nazwę kanału i wybierz "Ustawienia kanału".
4. Przejdź do zakładki **Integracje** > **Webhooki**.
5. Stwórz nowy webhook i skopiuj jego URL.
6. Wklej URL webhooka w pliku konfiguracyjnym programu **UNIC V2 RV**.

## Przykład pliku konfiguracyjnego

```json
{
    "discord_webhook_url": "https://discord.com/api/webhooks/your-webhook-url",
    "delete_temp_files": true,
    "delete_cache_files": true,
    "delete_log_files": true
}
