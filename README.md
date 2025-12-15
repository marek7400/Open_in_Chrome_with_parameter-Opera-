# Open in Chrome (Opera extension) / Otwórz w Chrome

[English](#english) | [Polski](#polski)

---

<a name="english"></a>
## 🇬🇧 English

I used an extension created by someone else for a long time. At some point, I needed to run Chrome, but with a specific parameter so that the uBlock Origin extension would still work. The old extension wouldn't work even though I entered the correct data, so I wrote my own version.

### Description
This extension allows you to open the current tab in a new Chrome instance with the following flags (defined in `host.js`):
```text
--disable-features=ExtensionManifestV2Unsupported,ExtensionManifestV2Disabled
Installation
1. Load the Extension
Open Chrome and navigate to chrome://extensions.
Enable Developer mode (toggle the switch in the top right corner).
Click Load unpacked.
Select the extension folder (chrome_launcher_extension).
2. Configure the Native Host
Note the ID of the newly loaded extension (a long string of characters like abcdef...).
Open the extension folder on your computer.
Double-click setup.bat.
Run it (you might need to accept Windows security warnings as it runs a script).
Paste the Extension ID when prompted and press Enter.
3. Usage
Click the blue/white extension icon in your Chrome/Opera toolbar.
The current page should open in a new Chrome window with the legacy flags applied.
Troubleshooting
Nothing happens? Ensure you have Node.js installed and in your PATH (see instructions below).
Debugging: Open host/host.bat and add pause at the end to see if it returns an error when run manually (note: it expects stdin input during normal operation).
Logs: Check background.js console logs. Go to the extensions page, click "Inspect views: background page" (or similar) and look for "Native Messaging" errors.
📘 Appendix: Installing Node.js on Windows 10
1. Go to the official website
Open your browser and go to: https://nodejs.org
2. Select the version
Download the LTS (Long Term Support) version – it is the most stable and recommended for most users.
3. Download and Run the installer
Click the Windows Installer (.msi) button.
Save the file and double-click it to run.
If the User Account Control prompt appears, select Yes.
4. Installation process
Click Next.
Accept the license terms.
Select the installation folder (default is recommended).
Leave the default options (Node.js, npm, Add to PATH) selected.
(Optional) You can select "Tools for Native Modules" if you need them, but it is not required for this extension.
5. Finish
Click Install.
When finished, click Finish.
6. Verify the installation
Open Command Prompt (cmd) or PowerShell.
Type:
code
Bash

download

content_copy

expand_less
node -v
npm -v
If version numbers appear, the installation was successful.
<a name="polski"></a>
🇵🇱 Polski
Długo używałem rozszerzenia zrobionego przez kogoś. W pewnym momencie zaszła potrzeba uruchomienia Chrome, ale z zadanym parametrem, żeby wciąż działało rozszerzenie uBlock Origin. Stare rozszerzenie mimo wpisania poprawnych danych nie chciało działać, dlatego napisałem własną wersję.
Opis
To rozszerzenie umożliwia otwarcie bieżącej karty w nowej instancji przeglądarki Chrome z następującymi flagami (wpisane w pliku host.js):
code
Text

download

content_copy

expand_less
--disable-features=ExtensionManifestV2Unsupported,ExtensionManifestV2Disabled
Instalacja
1. Załaduj rozszerzenie
Otwórz przeglądarkę Chrome i przejdź do chrome://extensions.
Włącz tryb programisty (przełącznik w prawym górnym rogu).
Kliknij Załaduj rozpakowane.
Wybierz ten folder (chrome_launcher_extension).
2. Skonfiguruj natywny host
Zanotuj identyfikator (ID) nowo załadowanego rozszerzenia (długi ciąg znaków, np. abcdef...).
Otwórz folder z rozszerzeniem na dysku.
Kliknij dwukrotnie plik setup.bat.
Uruchom go (może być konieczne zaakceptowanie ostrzeżeń zabezpieczeń systemu Windows, ponieważ uruchamia on skrypt).
Wklej ID po wyświetleniu monitu i naciśnij Enter.
3. Sposób użycia
Kliknij niebiesko-białą ikonę rozszerzenia na pasku narzędzi Chrome/Opera.
Bieżąca strona powinna otworzyć się w nowym oknie Chrome z zastosowanymi flagami starszej wersji.
Rozwiązywanie problemów
Nic się nie dzieje? Upewnij się, że masz zainstalowany Node.js i znajduje się on w ścieżce PATH (instrukcja poniżej).
Debugowanie: Otwórz plik host/host.bat i dodaj pause na końcu, aby sprawdzić, czy podczas ręcznego uruchamiania pojawia się błąd (chociaż skrypt oczekuje danych wejściowych stdin).
Logi: Sprawdź logi konsoli background.js. Na stronie rozszerzeń kliknij podgląd strony w tle (background page) i szukaj błędów „Native Messaging”.
📘 Dodatek: Instalacja Node.js na Windows 10 – krok po kroku
1. Wejście na stronę oficjalną
Otwórz przeglądarkę i przejdź na stronę: https://nodejs.org
2. Wybór wersji
Pobierz wersję LTS (Long Term Support) – jest najbardziej stabilna i zalecana dla większości użytkowników.
3. Pobranie i uruchomienie instalatora
Kliknij przycisk Windows Installer (.msi).
Zapisz plik na dysku i uruchom go dwukrotnym kliknięciem.
Jeśli pojawi się komunikat Kontroli konta użytkownika, wybierz Tak.
4. Przebieg instalacji
Kliknij Next.
Zaakceptuj licencję (I accept the terms…).
Wybierz folder instalacji (domyślny jest zalecany).
Pozostaw domyślne opcje (Node.js, npm, Add to PATH).
(Opcjonalnie) Możesz zaznaczyć opcję instalacji Tools for Native Modules, ale nie jest to wymagane dla tego rozszerzenia.
5. Zakończenie instalacji
Kliknij Install.
Po zakończeniu kliknij Finish.
6. Sprawdzenie poprawności instalacji
Otwórz Wiersz polecenia lub PowerShell.
Wpisz:
code
Bash

download

content_copy

expand_less
node -v
npm -v
Jeśli pojawią się numery wersji, instalacja zakończyła się sukcesem. Node.js i npm są gotowe do użycia.
