# Go-Projekt: Einfaches ausführbares Programm

## Beschreibung

Das hier gezeigte Beispielprojekt kann als Basis bzw. Kopiervorlage für
ein einfaches ausführbares Programm verwendet werden, das z.B. mit dem
Benutzer über die Konsole interagiert.

Es gibt hier nur zwei Dateien:

* `main.go`: Eine Go-Quelldatei mit einer Funktion `main()`.
  * Es ist nicht notwendig, dass diese Datei `main.go` heißt,
    eine beliebige Textdatei genügt, deren Name auf `.go`
    (aber nicht auf `_test.go`) endet.
  * Der Inhalt dieser Datei muss das Package `main` definieren
    und eine Funktion `main()` enthalten. Es dürfen beliebige weitere
    Funktionen enthalten sein.
* `go.mod`: Eine Textdatei, in der Metadaten zum Projekt spezifiziert werden.
            Der Inhalt dieser Datei ist i.W. eine Formalität, mehr dazu unten.

Diese Datei (`README.md`) gehört nicht zum Projekt bzw. sie ist nicht notwendig,
um ein Go-Programm zu schreiben.

## Verwendung

Dieses Minimalprojekt kann als Kopiervorlage benutzt werden.
Ein beliebiger Ordner mit diesen beiden Dateien ist ein Go-Projekt.
Falls Sie Visual Studio Code verwenden und Go installiert haben,
können Sie diesen Ordner mit VSCode öffnen und benutzen.

Beim ersten Verwenden einer Go-Quelldatei wird VSCode noch fragen,
ob es die benötigten Plugins und Erweiterungen installieren soll.
Nachdem dies erledigt ist, kann das Projekt verwendet werden und
wird von VSCode "verstanden".

Eine andere Entwicklungsumgebung für Go wird ggf. ein eigenes Projekt
konfigurieren und weitere Dateien hineinlegen, sie wird aber auch mit
diesem Ordner umgehen können.

## Erklärung zu go.mod

Diese Datei enthält eine Zeile mit dem Namen des Go-Moduls, das hier
erstellt wird. Falls das Projekt nicht öffentlich ist, spielt dieser Name
keine Rolle, er muss lediglich eindeutig sein.
D.h. falls man einen Workspace mit mehreren Modulen hat, darf dieser Name
nicht mehrfach vorkommen.

Ist das Projekt öffentlich, sollte dieser Modulname der Url entsprechen, unter der das
Projekt auffindbar ist.

Außerdem enthält diese Datei noch die Go-Version, mit der dieses Projekt erstellt wurde.
Falls komplexere Sprach-Features verwendet werden, kann dies bedeuten, dass diese
Go-Version auch benötigt wird, um das Projekt zu verwenden.
