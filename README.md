# PASSSAFE

English     (Deutsch weiter unten)



A private password manager for Windows, your browser and your Android
phone. Your data stays in files you control (for example in a Dropbox folder).
No account, no cloud service of mine, no tracking.

Free. If it is useful to you, you can buy me a coffee.





# ===========


ENGLISH
===

## WHAT'S INCLUDED

1. Desktop app (Windows)
Manage your entries: title, category, URL, username, email, phone,
password, one-time code (2FA) and notes. Search, categories, password
generator, dark theme, tray icon.
2. Browser extension (Chrome, Edge, other Chromium browsers)
Fills in the login of the website you are visiting, including the
one-time code.
3. Android app (read-only viewer)
Open your encrypted file, enter your master password, view entries, copy
values and see live one-time codes.



## FEATURES

* Choose what is typed as the login: per entry you pick Username, Email or
Phone (Edit -> "Browser login"). In the extension popup you can also click
the value you want right before filling.
* Optional encryption: switch "Encrypted" ON and your data is stored in
passsafe\_encrypted.json, protected by your master password (scrypt key
derivation + AES-256-GCM). The button is green when encryption is on and
red when it is off.
* One-time codes (TOTP): store the secret key and see
the current code in the app, the extension and on the phone.
* Same data everywhere: the data files live next to the program. Put the
whole folder in Dropbox (or another synced folder) to use it on several PCs
and on your phone.
* The Android app is locked down: no internet permission, screenshots are
blocked, and it locks when you tap "Lock".



## INSTALLATION

1. Desktop app
a) Download the installer and run it.
b) Start Passsafe and create your entries. Turn "Encrypted" ON and set a
master password if you want encryption.
2. Browser extension
a) Open chrome://extensions (or edge://extensions) and turn on
"Developer mode".
b) Click "Load unpacked" and select the "passsafe-extension" folder.
c) Start Passsafe, click "Browser..." and copy the pairing code.
d) Click the extension icon -> "Open settings", paste the code and save.
e) Use it: click the extension icon on a login page and pick an entry,
or press Alt+Shift+L to fill the first entry that matches the site.
3. Android app
a) Copy passsafe-viewer.apk to your phone (for example via Dropbox) and
open it.
b) Android asks you to allow installing from this source; confirm. Google
Play Protect may show a warning for apps from outside the Play Store.
c) Open the app, tap "Open your Passsafe file", choose
passsafe\_encrypted.json (for example from Dropbox) and enter your
master password.
The app only shows data. Make changes in the desktop app and let Dropbox
sync before you open the file on the phone.



## YOUR DATA FILES

Everything is stored in the folder where passsafe.py / the program is
installed:

passsafe\_encrypted.json  Your data, encrypted with the master password
(used when "Encrypted" is ON).
passsafe.json            Your data in PLAIN TEXT (used when "Encrypted" is
OFF).
passsafe\_browser.json    Pairing code for the browser extension.

On start, the newer of the two data files is loaded.

IMPORTANT: After turning encryption on, delete the old passsafe.json from
synced folders such as Dropbox. They still contain your passwords in plain text.



## SECURITY NOTES

* The browser extension talks only to the desktop app on your own computer,
using the pairing code.
* Your data leaves your devices only if you put the files into a cloud folder
yourself.
* If you forget your master password, encrypted data CANNOT be recovered.
Keep a backup.



## REQUIREMENTS

Windows PC, Chrome/Edge or another Chromium browser, Android 6.0 or newer
(for the phone app).



## LICENSE AND DISCLAIMER

Provided "as is", without warranty of any kind.





# ===========


DEUTSCH
===

Ein privater Passwort-Manager für Windows, deinen Browser und dein
Android-Handy. Deine Daten liegen in Dateien, die du selbst kontrollierst (zum
Beispiel in einem Dropbox-Ordner). Kein Konto, kein Cloud-Dienst von mir, kein
Tracking.

Kostenlos. Wenn es dir nützt, kannst du mir einen Kaffee spendieren.



## DAS IST ENTHALTEN

1. Desktop-Programm (Windows)
Einträge verwalten: Titel, Kategorie, URL, Benutzername, E-Mail, Telefon,
Passwort, Einmalcode (2FA) und Notizen. Suche, Kategorien,
Passwort-Generator, dunkles Design, Tray-Symbol.
2. Browser-Erweiterung (Chrome, Edge, andere Chromium-Browser)
Trägt das Login der besuchten Webseite ein, auch den Einmalcode.
3. Android-App (reiner Viewer)
Verschlüsselte Datei öffnen, Master-Passwort eingeben, Einträge ansehen,
Werte kopieren und Einmalcodes live anzeigen.



## FUNKTIONEN

* Du bestimmst, was als Login eingetragen wird: pro Eintrag wählst du
Username, Email oder Phone. Im Popup der Erweiterung kannst du den
gewünschten Wert auch direkt vor dem Ausfüllen anklicken.
* Verschlüsselung (optional): Schaltest du "Encrypted" auf ON, werden die
Daten in passsafe\_encrypted.json gespeichert, geschützt durch dein
Master-Passwort (scrypt-Schlüsselableitung + AES-256-GCM). Der Button ist
grün, wenn die Verschlüsselung an ist, und rot, wenn sie aus ist.
* Einmalcodes (TOTP): Speicher den Schlüssel im PC und benutze den aktuellen
Code in der Erweiterung und auf dem Handy.
* Überall dieselben Daten: Die Datendateien liegen im Programm-Ordner. Lege
den ganzen Ordner in Dropbox (oder einen anderen synchronisierten Ordner),
um ihn auf mehreren PCs und auf dem Handy zu nutzen.
* Die Android-App ist abgesichert: keine Internet-Berechtigung, Screenshots
gesperrt, und sie sperrt wenn du auf "Lock" tippst.



## INSTALLATION

1. Desktop-Programm
a) Installer herunterladen und ausführen.
b) Passsafe starten und deine Einträge anlegen. Wenn du Verschlüsselung
willst, "Encrypted" auf ON stellen und ein Master-Passwort vergeben.
2. Browser-Erweiterung
a) chrome://extensions (oder edge://extensions) öffnen und den
"Entwicklermodus" einschalten.
b) "Entpackte Erweiterung laden" anklicken und den Ordner
"passsafe-extension" auswählen.
c) Passsafe starten, auf "Browser..." klicken und den Kopplungscode
kopieren.
d) Auf das Erweiterungs-Symbol klicken -> "Open settings", Code einfügen
und speichern.
e) Benutzen: Auf einer Login-Seite auf das Symbol klicken und einen Eintrag
wählen, oder Alt+Shift+L drücken, um den ersten passenden Eintrag
auszufüllen.
3. Android-App
a) passsafe-viewer.apk aufs Handy übertragen (zum Beispiel über Dropbox) und
öffnen.
b) Android fragt, ob das Installieren aus dieser Quelle erlaubt ist;
bestätigen. Google Play Protect kann bei Apps von außerhalb des Play
Stores eine Warnung zeigen.
c) App öffnen, "Open your Passsafe file" antippen, passsafe\_encrypted.json
auswählen (zum Beispiel aus Dropbox) und das Master-Passwort eingeben.
Die App zeigt nur Daten an. Änderungen machst du im Desktop-Programm;
warte, bis Dropbox synchronisiert hat, bevor du die Datei auf dem Handy
öffnest.



## DEINE DATENDATEIEN

Alles liegt im Ordner, in dem passsafe.py bzw. das Programm installiert ist:

passsafe\_encrypted.json  Deine Daten, mit dem Master-Passwort verschlüsselt
(wird bei "Encrypted" ON benutzt).
passsafe.json            Deine Daten im KLARTEXT (wird bei "Encrypted" OFF
benutzt).
passsafe\_browser.json    Kopplungscode für die Browser-Erweiterung.

Beim Start wird die neuere der beiden Datendateien geladen.

WICHTIG: Lösche nach dem Einschalten der Verschlüsselung die alte
passsafe.json (und alte Sicherungen wie passsafe\_old\_...json) aus
synchronisierten Ordnern wie Dropbox. Dort stehen deine Passwörter weiterhin
im Klartext.



## SICHERHEITSHINWEISE

* Die Browser-Erweiterung spricht nur mit dem Desktop-Programm auf deinem
eigenen Rechner, über den Kopplungscode.
* Deine Daten verlassen deine Geräte nur, wenn du die Dateien selbst in einen
Cloud-Ordner legst.
* Wenn du das Master-Passwort vergisst, lassen sich verschlüsselte Daten NICHT
wiederherstellen. Lege ein Backup an.



## VORAUSSETZUNGEN

Windows-PC, Chrome/Edge oder ein anderer Chromium-Browser, Android 6.0 oder
neuer (für die Handy-App).



## LIZENZ UND HAFTUNGSAUSSCHLUSS

Bereitgestellt "wie besehen", ohne jegliche Gewährleistung.

