# ****Basis Einleitung in**** C****

### C ist eine prozedurale Programmiersprache, die direkten Zugriff auf Speicher ermöglicht. Sie wird für Systemprogrammierung, Spiele, Treiber und vieles mehr verwendet. C-Code wird direkt in Maschinencode übersetzt und ist somit in der Praxis schneller als interpretierter Code.

## ****K**ompilierte und Interpretierte sprachen**

Bei Kompilierten Sprachen wird der Code direkt in Maschinencode
übersetzt was den Vorteil trägt, dass der Code schneller ist und über
eine engere Hardwarekontrolle verfügt. Bei Interpretierten Sprachen wird
der Code Zeile für Zeile oder in kleinen Blöcken interpretiert und
ausgeführt. Das Interpretieren bringt als Vorteil eine
Plattformunabhängigkeit und Flexibilität.

## **Anwendung**

Die Programmiersprache C findet in vielen Bereichen der Informatik und
Technik Anwendung und gehört zu den wichtigsten und langlebigsten
Sprachen überhaupt. Sie wird vor allem dort eingesetzt, wo es auf
Effizienz, Geschwindigkeit und direkten Zugriff auf die Hardware
ankommt.

## 

## Compiler Installieren

### Windows

Um C-Programme auf Windows zu schreiben und zu kompilieren, benötigst du
einen ****C-Kompiler****. Eine der besten Optionen ist
****MinGW-w64****, weil es leichtgewichtig ist und gut mit vielen
Entwicklungsumgebungen funktioniert.

#### ****Schritt 1: MinGW-w64 herunterladen****

1.  Öffne die offizielle MinGW-w64 Download-Seite:\
    <https://winlibs.com/>
2.  Lade die ****Latest MinGW-w64 GCC Build**** herunter (z. B. „UCRT
    Runtime, Win64").
3.  Entpacke die ZIP-Datei an einen festen Speicherort (z. B.
    **C:\\mingw64**).

#### ****Schritt 2: Umgebungsvariablen setzen****

Damit Windows den Kompiler von überall aus erkennt:

1.  Öffne die ****Einstellungen**** → ****System**** → ****Erweiterte
    Systemeinstellungen****.
2.  Klicke auf ****Umgebungsvariablen****.
3.  Wähle im unteren Bereich die Variable ****Path**** und klicke auf
    ****Bearbeiten****.
4.  Klicke auf ****Neu**** und füge den Pfad zu **C:\\mingw64\\bin**
    hinzu.
5.  Bestätige mit ****OK**** und starte dein Terminal neu.

#### ****Schritt 3: Installation testen****

Öffne die ****Eingabeaufforderung (CMD)**** oder ****PowerShell**** und
tippe:

*gcc \--version*

Wenn eine Version ausgegeben wird (z. B. **gcc (MinGW-w64) x.x.x**), ist
die Installation erfolgreich!

### Linux

**Unter Linux ist die Installation in der Regel ******einfacher******,
hängt aber von der verwendeten ******Distribution****** ab.**

#### Debian/Ubuntu (APT-basiert)

*sudo apt update*

#### ****

## **Hello World in C**

### ****Programm schreiben****

****Um unseres klassische Hello World können wir natürlich auch in C
schreiben. Dafür braucht man nur einen Code Editor und ein file, dass z.
b. hello.c heisst. ****Und dann schreiben wir folgendes rein:****

#include \<stdio.h\>

int main() {

printf(\"Hello, World!\\n\");

return 0;

}

#include \<stdio.h\>

### #Include sagt dem Programm: \"Benutze die Funktionen aus der Bibliothek stdio.\" Diese Bibliothek enthält Funktionen für die Ein- und Ausgabe -- z. B. printf().

int main() {

Jedes C-Programm beginnt mit der Funktion main().\
int bedeutet, dass die Funktion am Ende eine Zahl (vom Typ „Integer")
zurückgibt.

printf(\"Hello, World!\\n\");

printf() ist eine Funktion, die etwas ins Terminal schreibt.\
\"Hello, World!\\n\" ist der Text -- \\n steht für einen Zeilenumbruch.

return 0;

}

return 0; beendet das Programm und gibt den Wert 0 an das Betriebssystem
zurück.\
Das bedeutet: „Alles ist gut gelaufen."\
Die schliessende Klammer } beendet die main-Funktion.

### 

### Programm Kompilieren

****Die meisten Windows-Nutzer haben vorher noch nie mit einer
****Shell**** gearbeitet. Keine Sorge -- das ist einfacher als es
klingt.****

#### ****Windows****

Schritt 1: PowerShell öffnen

1.  Drücke **Windows-Taste**
2.  Tippe **PowerShell**
3.  Klicke auf **Windows PowerShell** (oder „Terminal", wenn du Windows
    11 nutzt)

Du erkennst PowerShell am blauen Fenster mit dem Prompt **PS
C:\\\...\>**.

Schritt 2: In den Ordner wechseln

Wechsle in den Ordner, in dem deine **.c**-Datei liegt, z. B.:

****cd C:\\Users\\DeinName\\Documents\\C-Projekte****

****Vergewissere dich mit:****

****dir****

****... ****dass die Datei hello.c im Verzeichnis liegt.****

**Schritt 3: Programm kompilieren**

****Gib folgenden Befehle ein:****

****gcc hello.c -o hello.exe****

****Erklärung:****

-   **gcc** startet den Compiler
-   **hello.c** ist dein Quellcode
-   **-o hello.exe** bedeutet: Die Ausgabedatei heisst **hello.exe**

#### **Schritt 4: Programm ausführen**

Jetzt kannst du dein Programm direkt starten mit:

*.\\hello.exe*

**Du solltest deine Ausgabe im PowerShell-Fenster sehen **mit**
**„Hello, World!"**.**

#### **Linux**

****Auf Linux ist der Ablauf sehr ähnlich, aber statt PowerShell nutzt
man das Terminal:****

****gcc hello.c -o hello****

****./hello****

****Hinweis: Unter Linux heissen ausführbare Dateien normalerweise
****einfach ******hello******, ohne ******.exe******.****

## ****Fazit****

C ist eine leistungsstarke, effiziente und hardwarenahe
Programmiersprache, die bis heute in vielen Bereichen der
Softwareentwicklung unverzichtbar ist. Sie bietet volle Kontrolle über
Speicher und Rechenleistung, ist plattformunabhängig und bildet die
Grundlage vieler moderner Systeme und Sprachen. Wer C lernt, versteht
nicht nur das Programmieren besser, sondern auch, wie Computer wirklich
funktionieren
