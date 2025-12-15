
[English](#english) | [Polski](#polski)

---

<a name="english"></a>

I used an extension created by someone else for a long time.
At some point, I needed to run Chrome, but with a specific parameter so that theuBlock Origin extension would still work.
The old extension wouldn't work even though I entered the correct data, so I wrote my own version.

# Open in Chrome (Opera extension)

This extension allows you to open the current tab in a new Chrome instance with the following flags:
`--disable-features=ExtensionManifestV2Unsupported,ExtensionManifestV2Disabled`
(in file host.js)

## Installation

1. **Load the Extension**:
   - Open Chrome and go to `chrome://extensions`.
   - Enable **Developer mode** (top right switch).
   - Click **Load unpacked**.
   - Select this folder (`chrome_launcher_extension`).

2. **Configure the Native Host**:
   - Note the **ID** of the newly loaded extension (a long string of characters like `abcdef...`).
   - Double-click `setup.bat` in this folder.
   - Run it (you might need to accept Windows security warnings as it runs a script).
   - Paste the **ID** when prompted and press Enter.

3. **Usage**:
   - Click the blue/white extension icon in your Chrome toolbar.
   - The current page should open in a new Chrome window with the legacy flags applied.

## Troubleshooting
- If nothing happens, ensure you have **Node.js** installed and in your PATH.
- Open `host/host.bat` and add `pause` at the end to see if it errors when run manually (though it expects stdin input).
- Check `background.js` console logs (Inspect the extension background page) for "Native Messaging" errors.
--------------------------------------------------------------------------------
Installing Node.js on Windows 10 – step by step (in points):

Go to the official website

Open your browser and go to: https://nodejs.org

Selecting the version

Download the LTS (Long Term Support) version – it is the most stable and recommended for most users

Downloading the installer

Click the Windows Installer (.msi) button

Save the file to your hard drive

Running the installer

Double-click the downloaded .msi file

If the User Account Control prompt appears, select Yes

Installation process

Click Next

Accept the license (I accept the terms…)

Select the installation folder (the default is recommended)

Leave the default options (Node.js, npm, Add to PATH)

Installing additional tools

You can select the Tools for Native Modules installation option (optional, useful for some packages)

Completing the installation

Click Install

When finished, click Finish

Verifying the installation

Open Command Prompt or PowerShell

Type:

node -v


Then:

npm -v


If version numbers appear, the installation was successful

Ready to go

Node.js and npm are ready to use

You can create and run JavaScript applications

--------------------------------------------------------------------------------
<a name="polski"></a>
🇵🇱 Polski

Open in Chrome (Opera extension)

Długo używałem rozszerzenia zrobionego przez kogoś.
W pewnym momencie zaszła potrzeba uruchomienia Chrome, ale z zadanym parametrem,żeby wciąż działało rozszerzenie uBlock Orgin.
Stare rozszerzenie mimo wpisania poprawnych danych nie chciało działać, dlatego napisałem własną wersję.
***
To rozszerzenie umożliwia otwarcie bieżącej karty w nowej instancji przeglądarki Chrome z następującymi flagami:

`--disable-features=ExtensionManifestV2Unsupported,ExtensionManifestV2Disabled`
(wpisane w pliku host.js)

## Instalacja

1. **Załaduj rozszerzenie**:

   - Otwórz przeglądarkę Chrome i przejdź do `chrome://extensions`.

   - Włącz **tryb programisty** (przełącznik w prawym górnym rogu).

   - Kliknij **Załaduj rozpakowane**.

   - Wybierz ten folder (`chrome_launcher_extension`).

2. **Skonfiguruj natywny host**:

   - Zanotuj **identyfikator** nowo załadowanego rozszerzenia (długi ciąg znaków, np. `abcdef...`).

   - Kliknij dwukrotnie plik `setup.bat` w tym folderze.

   - Uruchom go (może być konieczne zaakceptowanie ostrzeżeń zabezpieczeń systemu Windows, ponieważ uruchamia on skrypt).

   - Wklej **ID** po wyświetleniu monitu i naciśnij Enter.

3. **Sposób użycia**:

   - Kliknij niebiesko-białą ikonę rozszerzenia na pasku narzędzi Chrome.

   - Bieżąca strona powinna otworzyć się w nowym oknie Chrome z zastosowanymi flagami starszej wersji.

## Rozwiązywanie problemów

- Jeśli nic się nie dzieje, upewnij się, że masz zainstalowany **Node.js** i znajduje się on w ścieżce PATH.

- Otwórz plik `host/host.bat` i dodaj `pause` na końcu, aby sprawdzić, czy podczas ręcznego uruchamiania pojawia się błąd (chociaż oczekuje on danych wejściowych stdin).

- Sprawdź logi konsoli `background.js` (sprawdź stronę rozszerzenia w tle) pod kątem błędów „Native Messaging”.
--------------------------------------------------------------------------------
Instalacja Node.js na Windows 10 – krok po kroku (w punktach):

Wejście na stronę oficjalną

Otwórz przeglądarkę i przejdź na stronę: https://nodejs.org

Wybór wersji

Pobierz wersję LTS (Long Term Support) – jest najbardziej stabilna i zalecana dla większości użytkowników

Pobranie instalatora

Kliknij przycisk Windows Installer (.msi)

Zapisz plik na dysku

Uruchomienie instalatora

Kliknij dwukrotnie pobrany plik .msi

Jeśli pojawi się komunikat Kontroli konta użytkownika, wybierz Tak

Przebieg instalacji

Kliknij Next

Zaakceptuj licencję (I accept the terms…)

Wybierz folder instalacji (domyślny jest zalecany)

Pozostaw domyślne opcje (Node.js, npm, Add to PATH)

Instalacja dodatkowych narzędzi

Możesz zaznaczyć opcję instalacji Tools for Native Modules (opcjonalnie, przydatne do niektórych pakietów)

Zakończenie instalacji

Kliknij Install

Po zakończeniu kliknij Finish

Sprawdzenie poprawności instalacji

Otwórz Wiersz polecenia lub PowerShell

Wpisz:

node -v


Następnie:

npm -v


Jeśli pojawią się numery wersji, instalacja zakończyła się sukcesem

Gotowość do pracy

Node.js i npm są gotowe do użycia

Możesz tworzyć i uruchamiać aplikacje JavaScript

