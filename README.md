

<div id="texts" style="display:inline; white-space:nowrap; float: right;"> 
        <h1>Visual Studio mit Git und GitHub</h1>
</div>

## :dart: Zielsetzung

### 1. Verständnis für die Entwicklungsumgebung
- Die Lernenden können **Visual Studio 2022** erfolgreich installieren, starten und die wichtigsten Funktionen der IDE identifizieren.

### 2. Anwendung von Versionierungssystemen
- Die Lernenden sind in der Lage, ein Projekt in Visual Studio zu erstellen und dieses mit einem Git-Repository zu verbinden.
- Sie verstehen die Bedeutung von Commits und können diese in Visual Studio durchführen.

### 3. Zusammenarbeit mit GitHub
- Die Lernenden können sich mit ihren Konten in Visual Studio anmelden.
- Sie können ein neues Repository auf GitHub erstellen, Änderungen pushen und ziehen (fetch und pull).
- Sie verstehen den Unterschied zwischen diesen Aktionen.

### 4. Arbeiten mit C#-Projekten
- Die Lernenden sind in der Lage, ein neues C#-Konsolenprojekt in Visual Studio zu erstellen.
- Sie können bestehende Projekte bearbeiten und verschiedene Projekte innerhalb einer Lösung verwalten.


## Einleitung

Die Integration von Visual Studio mit GitHub hat die Entwicklung und Zusammenarbeit von Software erheblich vereinfacht. In diesem Tutorial werden Sie durch den Prozess der Erstellung eines Projekts in Visual Studio 2022 geführt, seiner Verbindung mit einem GitHub-Repository und der Durchführung der grundlegenden Git-Operationen, die im Softwareentwicklungszyklus häufig verwendet werden. Nachdem Sie diesen Leitfaden befolgt haben, werden Sie über das notwendige Wissen verfügen, um Ihren Code effizient zu verwalten, Änderungen zu verfolgen und mit anderen Entwicklern zusammenzuarbeiten.

---


## Visual Studio Starten

Um Visual Studio 2022 zu starten, folgen Sie diesen einfachen Schritten:

1. Öffnen Sie die Windows-Suchleiste und geben Sie "Visual Studio 2022" ein.

<img src="./AddFiles/Suchleiste-windows.PNG" width=50% >

2. Wählen Sie das entsprechende Suchergebnis aus, indem Sie darauf klicken.

3. Sollte ein Popup-Fenster erscheinen, klicken Sie auf **"ohne Code fortfahren"**.

<img src="./AddFiles/startbildschirm.PNG" width=50% >

## Kontoeinstellungen in Visual Studio 2022

Bevor Sie mit der Arbeit in Visual Studio 2022 beginnen, ist es wichtig, Ihr **Microsoft-Konto** und Ihr **GitHub-Konto** zu verknüpfen. Ein Microsoft-Konto ermöglicht Ihnen den Zugriff auf verschiedene Dienste von Microsoft und sichert Ihre Einstellungen in der Cloud. Ein GitHub-Konto wird benötigt, wenn Sie Ihre Projekte versionieren und online auf GitHub speichern möchten.

### 1. **Account anmelden**

- Navigieren Sie im Menü zu `Datei` > `Kontoeinstellungen`.

<img src="./AddFiles/Datei-Kontoeinstellungen.png" width=50% >

- Klicken Sie auf **"Anmelden"** und geben Sie Ihre Schul-E-Mail-Adresse ein, um sich bei Ihrem **Microsoft-Konto** anzumelden.

<img src="./AddFiles/Anmelden-Microsoft.PNG" width=50% >

> **Hinweis**: Sollten Probleme bei der Anmeldung auftreten, wechseln Sie den Standardbrowser in den `Kontooptionen`.


<img src="./AddFiles/Anmeldeoption.png" width=50% >

### 2. **GitHub Konto hinzufügen**

- Nachdem Sie sich mit Ihrem Microsoft-Konto angemeldet haben, fügen Sie Ihr **GitHub-Konto** hinzu.
- Klicken Sie hierfür auf **"Hinzufügen"** und wählen Sie GitHub aus der Liste aus.


<img src="./AddFiles/GitHub-Anmeldung.png" width=50% >


Nach erfolgreicher Anmeldung mit beiden Konten sollte Ihr Anmeldebildschirm wie folgt aussehen:


<img src="./AddFiles/Angemeldet.PNG" width=50% >

## Neue Projektmappe in Visual Studio 2022 erstellen

In diesem Abschnitt werden Sie lernen, wie Sie eine neue Projektmappe für ein Konsolenprogramm erstellen, das in der Programmiersprache **C#** geschrieben wird. Ein **Konsolenprogramm** ist eine Art von Anwendung, die in einem Konsolenfenster (auch bekannt als Befehlszeilenfenster) ausgeführt wird. Es besitzt keine grafische Benutzeroberfläche (GUI), stattdessen interagiert es mit dem Benutzer durch Texteingaben und -ausgaben.

### 1. **Projekt erstellen**

- Navigieren Sie im Menü zu `Datei` > `Neu` > `Projekt`.

<img src="./AddFiles/Neues-Projekt.png" width=50% >

- Geben Sie in die Suchleiste `Konsolen.App` ein und stellen Sie sicher, dass **C#** als gewählte Programmiersprache eingestellt ist.

<img src="./AddFiles/Neues-Konsolenprojekt.PNG" width=50% >

### 2. **Projekt konfigurieren**

- Benennen Sie die Projektmappe im ersten Feld als **"GrundlagenrepositoryCsharp"** und das darin enthaltene Projekt als **"1_Elementare_Syntax"** im zweiten Feld.
- Es ist eine gängige Praxis, Repositorys im `source` Ordner des Benutzers zu speichern. Achten Sie darauf, die Projektmappe **nicht** im selben Verzeichnis wie das Projekt zu platzieren.

<img src="./AddFiles/Projektnamen-festlegen.PNG" width=50% >

- Für dieses Tutorial wählen Sie die Framework-Version **.NET 6**.

<img src="./AddFiles/Framework.PNG" width=50% >

Im Anschluss daran wird Visual Studio das Projekt initialisieren und Ihnen eine Übersicht über die erstellten Dateien und den Quellcode anzeigen.

## Projekt debuggen in Visual Studio 2022

Der **Debugger** ist ein essentielles Tool für Entwickler. Er ermöglicht es, den Programmcode Schritt für Schritt auszuführen, den Zustand von Variablen zu überwachen, Haltepunkte zu setzen und viele andere Aufgaben durchzuführen, die bei der Fehleridentifikation und -behebung helfen. Das Debuggen hilft dabei, das Verhalten und die Abläufe im Code besser zu verstehen, und ist daher ein unerlässliches Werkzeug bei der Softwareentwicklung.

### Debugger starten

- Um den Debugger zu starten, drücken Sie **F5** auf Ihrer Tastatur oder klicken Sie auf den grünen Pfeil in der Menüleiste.

<img src="./AddFiles/Debuggen.png" width=50% >

Nach dem Starten des Debuggers wird Ihr Code im Debug-Modus ausgeführt. Sie können den Verlauf des Programms verfolgen, Haltepunkte setzen und den Wert von Variablen während der Laufzeit beobachten. Dies ist besonders nützlich, um das korrekte Verhalten des Codes zu überprüfen und mögliche Fehler oder Unstimmigkeiten zu identifizieren.

### Neues Projekt in bestehende Projektmappe hinzufügen

In Visual Studio können Sie mehrere Projekte innerhalb einer einzigen **Projektmappe** organisieren. Dies ermöglicht es, mehrere miteinander verbundene Projekte zentral zu verwalten. Hier zeigen wir Ihnen, wie Sie ein neues Projekt zu einer bereits existierenden Projektmappe hinzufügen:

1. **Projektmappe im Solution Explorer auswählen**: 
    - Klicken Sie im Solution Explorer auf die lilafarbene Projektmappe, die Ihr Hauptprojekt enthält.

<img src="./AddFiles/Projektmappe.PNG" width=50% >

2. **Kontextmenü öffnen und neues Projekt hinzufügen**:
    - Klicken Sie mit der rechten Maustaste auf die ausgewählte Projektmappe und wählen Sie die Option, ein neues Projekt hinzuzufügen.

<img src="./AddFiles/Neues-Projekt-hinzu.png" width=50% >

3. **Projekteigenschaften festlegen**:
    - Geben Sie dem neuen Projekt den Namen **"2_Konsolenausgabe"**.
    - Achten Sie darauf, dass Sie das **.NET 6 Framework** als Zielplattform auswählen, um die Kompatibilität und Konsistenz zwischen Ihren Projekten sicherzustellen.

<img src="./AddFiles/Zweiter-Projektname.PNG" width=50% >

Nach Abschluss dieser Schritte ist das neue Projekt Ihrer bestehenden Projektmappe hinzugefügt und Sie können mit der Entwicklung innerhalb dieses neuen Projektes beginnen.

## Projekt zum Starten auswählen und ausführen

In einer **Projektmappe** mit mehreren Projekten in Visual Studio können Sie ein bestimmtes Projekt als Startprojekt festlegen. Das bedeutet, dass dieses Projekt beim Starten des Debuggers automatisch ausgeführt wird. Im Folgenden wird erläutert, wie Sie das Startprojekt ändern und überprüfen können, welche Ausgabe es erzeugt:

1. **Ändern des Quellcodes**:
    - Öffnen Sie die Datei `Program.cs` im neu hinzugefügten Projekt.
    - Ersetzen Sie den Text `Hello World` durch `Fubar`.
    - Speichern Sie die Datei.

<img src="./AddFiles/Änderung-zweites-Projekt.PNG" width=50% >


2. **Projekt ausführen und Ausgabe überprüfen**:
    - Starten Sie den Debugger, um die Ausgabe des aktuellen Startprojekts zu überprüfen.
    - Sie sollten die Ausgabe `Fubar` im Konsolenfenster sehen, wenn das aktuelle Startprojekt das neu hinzugefügte Projekt ist.

3. **Startprojekt ändern**:
    - Wenn Sie die Ausgabe von `Hello World` statt `Fubar` sehen, bedeutet dies, dass das ursprüngliche Projekt immer noch als Startprojekt festgelegt ist.
    - Um das neu hinzugefügte Projekt als Startprojekt festzulegen, klicken Sie mit der rechten Maustaste auf den Projektnamen im Solution Explorer.
    - Wählen Sie "Als Startprojekt festlegen" aus dem Kontextmenü.


<img src="./AddFiles/AlsStartprojekt-festlegen.png" width=50% >

4. **Erneutes Überprüfen der Ausgabe**:
    - Starten Sie den Debugger erneut.
    - Diesmal sollte die Ausgabe `Fubar` im Konsolenfenster angezeigt werden, da das neu hinzugefügte Projekt nun als Startprojekt festgelegt ist.

Indem Sie das Startprojekt wechseln, können Sie sicherstellen, dass Sie immer das richtige Projekt in Ihrer Projektmappe ausführen und testen.

### Ihr Projekt mit GitHub verbinden

Um sicherzustellen, dass Ihr Projekt von einer Versionskontrolle profitiert, ist es wichtig, es mit einem System wie GitHub zu verbinden. Dies ermöglicht es Ihnen, Änderungen nachzuverfolgen, mit anderen zusammenzuarbeiten und den Code sicher in der Cloud zu speichern.

1. **Initialisierung der Quellcodeverwaltung**:
    - Klicken Sie in Visual Studio auf die Schaltfläche **"Zur Quellcodeverwaltung hinzufügen"**.
    - Wählen Sie im daraufhin angezeigten Menü **"Git"** aus.

<img src="./AddFiles/Quellcodeverwaltung-hinzufügen.png" width=50% >

2. **Einige wichtige Einstellungen**:
    - Visual Studio bietet bereits einige vordefinierte Einstellungen. Überprüfen Sie die folgenden Punkte und passen Sie sie bei Bedarf an:

        - **README.md hinzufügen**: Eine `README.md`-Datei bietet allgemeine Informationen über Ihr Projekt und ist oft der erste Anhaltspunkt für andere Entwickler oder Nutzer, um zu verstehen, was Ihr Projekt macht und wie man es benutzt.

        - **Konto auswählen**: Stellen Sie sicher, dass Sie das richtige Konto auswählen, über das Sie das Repository erstellen möchten.

        - **Repository-Besitzer auswählen**: Wählen Sie, wem das Repository gehört. Wenn Sie Teil der GSO-Organisation sind, haben Sie die Möglichkeit, das Repository entweder Ihrem persönlichen Profil oder der Organisation zuzuweisen.

        - **Beschreibung hinzufügen**: Geben Sie eine kurze Beschreibung an, die den Inhalt und den Zweck des Repositories klar macht.

        - **Repository veröffentlichen**: Dieser Schritt erstellt das Repository auf GitHub. Beachten Sie, dass das Repository standardmäßig als **"Privat"** eingestellt ist, sodass nur Sie darauf Zugriff haben. Diese Einstellungen können später auf der GitHub-Website angepasst werden.


<img src="./AddFiles/repo-veröffentlichen.png" width=50% >

3. **Überprüfung auf GitHub**:
    - Nachdem Sie das Repository veröffentlicht haben, können Sie es direkt auf GitHub überprüfen. Melden Sie sich bei Ihrem GitHub-Konto an und navigieren Sie zu Ihrem persönlichen Profil. Hier sollte das neu erstellte Repository erscheinen.

    Mit diesen Schritten haben Sie Ihr Projekt erfolgreich in ein Git-Repository umgewandelt und dieses Repository auf GitHub veröffentlicht. Sie sind nun bereit, die Vorteile der Versionskontrolle und der Zusammenarbeit über GitHub zu nutzen.

### Synchronisation Ihrer lokalen Änderungen mit GitHub

Das Konzept von Git basiert auf der Trennung von lokalen und entfernten Repositories. Wenn Sie Änderungen in Ihrem lokalen Repository vornehmen, werden diese nicht automatisch auf das entfernte Repository (in diesem Fall auf GitHub) übertragen. Um diese Synchronisation durchzuführen, müssen Sie Ihre Änderungen "commiten" und dann "pushen".

1. **Fenster im Blick behalten**:
   - Es gibt zwei Hauptfenster in Visual Studio, die Sie beim Arbeiten mit Git oft nutzen werden:
      - Projektmappenexplorer: Zeigt die Struktur Ihrer Projekte.
      - Git-Änderungen: Zeigt alle Änderungen in Ihrem lokalen Repository.

<img src="./AddFiles/Ansicht-öffnen.png" width=50% >

Nun wollen Wir eine Änderung in der Program.cs des ersten Projekts (**"1_Elementare_Syntax"**) vornehmen. 
Schreiben Sie unter die Vorhandene Codezeile eine Übersetzung der Konsolenausgabe. 

```csharp
Console.WriteLine("Hello World");
Console.WriteLine("Hallo Welt");
```

<img src="./AddFiles/Bearbeitet.png" width=50% >

### Änderungen committen:

1. Klicken Sie auf die **"Git-Änderungen"-Registerkarte**.
2. Beschreiben Sie kurz und präzise, was Sie geändert haben. Eine gute Praxis ist es, aktive Verben zu verwenden (z.B. "hinzugefügt", "geändert").
3. Klicken Sie auf den **Commit-Button**, um Ihre Änderungen zu speichern.


<img src="./AddFiles/commit-lokal.png" width=50% >

### Warum ist meine Änderung nicht auf GitHub?:

Wenn Sie nach Ihrem Commit auf GitHub schauen, werden Sie feststellen, dass Ihre Änderungen noch nicht dort erscheinen. Das liegt daran, dass Commits zuerst lokal gespeichert werden. Um diese Änderungen auf das entfernte Repository zu übertragen, müssen Sie sie "pushen".

### Pushen Sie Ihre Änderungen:

1. Klicken Sie auf den **Pfeil-nach-oben-Button**, um Ihre Änderungen zu pushen. Die kleine Zahl neben dem Button zeigt an, wie viele Commits Sie seit dem letzten Push gemacht haben.
2. Nachdem der Push abgeschlossen ist, können Sie erneut auf GitHub nachsehen. Ihre Änderungen sollten jetzt im entfernten Repository sichtbar sein.

<img src="./AddFiles/erster-push.png" width=50% >

Durch diesen Prozess stellen Sie sicher, dass alle Ihre Änderungen sicher auf GitHub gespeichert sind und Sie oder andere Entwickler darauf von überall aus zugreifen können.

### Fetch und Pull

Während der Arbeit in einem Team oder durch Änderungen direkt im Browser kann es passieren, dass Änderungen am Code auf GitHub vorgenommen werden, die Sie noch nicht lokal auf Ihrem Rechner haben. Um diese Änderungen zu erhalten, müssen Sie diese zunächst "fetchen" und anschließend "pullen".

Führen Sie die folgenden Schritte aus, um eine Änderung im Browser vorzunehmen:

1. Gehen Sie in Ihrem Browser zu Ihrem Repository **GrundlagenrepositoryCsharp** und navigieren Sie zum Verzeichnis **2_Konsolenausgabe**.
2. Ersetzen Sie die Codezeile:
   ```csharp
   Console.WriteLine("Fubar");
   ```
   durch
   
        ```csharp
        Console.WriteLine("foobar");
        ```
Vergessen Sie nicht, Ihre Änderung zu committen.

<img src="./AddFiles/browser-commit.png" width=50% >

### Um die im Browser gemachten Änderungen lokal zu erhalten:

1. Öffnen Sie in Visual Studio die Registerkarte **Git-Änderungen**.
2. Klicken Sie auf den gestrichelten Pfeil nach unten, um die Daten abzurufen.
3. Visual Studio zeigt nun eine Änderung an, die online gemacht wurde. Beachten Sie: Diese Änderung ist lokal noch nicht übernommen!
4. Im Register "Eingehend" finden Sie den entsprechenden Commit.
5. Klicken Sie auf die Datei, in der der Commit gemacht wurde, um die Änderungen zu überprüfen.
6. Um die Änderung lokal zu übernehmen, klicken Sie erneut auf den Pfeil nach unten.

Überprüfen Sie abschließend, ob die Änderung auch lokal auf Ihrem Rechner übernommen wurde.

<img src="./AddFiles/fetch-pull.png" width=50% >

## Repository klonen

Ein Hauptgrund für die Speicherung von Code auf einem Server, wie z.B. GitHub, ist die Sicherung der Daten. Dies erlaubt es Ihnen und anderen, jederzeit auf den Code zuzugreifen und ihn zu verwenden, selbst wenn er lokal gelöscht wurde.

Befolgen Sie die folgenden Schritte, um zu erfahren, wie Sie ein gelöschtes Repository wiederherstellen können:

1. **Lokales Repository löschen:**
    - Schließen Sie Visual Studio.
    - Navigieren Sie zu dem Ordner, in dem Sie das **"GrundlagenrepositoryCsharp"** gespeichert haben.
    - Löschen Sie dieses Repository.

<img src="./AddFiles/Repository-löschen.png" width=50% >

2. **HTTPS-URL des Repositories kopieren:**
    - Öffnen Sie Ihren Browser und navigieren Sie zu Ihrem GitHub-Profil.
    - Klicken Sie auf das Repository **"GrundlagenrepositoryCsharp"**.
    - Klicken Sie auf den **'Code'**-Button und kopieren Sie die HTTPS-URL.

<img src="./AddFiles/url-klonen.png" width=50% >

3. **Repository mit Visual Studio klonen:**
    - Starten Sie Visual Studio.
    - Gehen Sie zu `Datei` und klicken Sie auf `Repository klonen`.
    

<img src="./AddFiles/repo-klonen.png" width=50% >

    - Fügen Sie die kopierte URL in das obere Feld ein.
    - Klicken Sie auf den `Klonen`-Button.


<img src="./AddFiles/klonen.png" width=50% >

Ihr Repository ist nun wieder auf Ihrem Computer und kann lokal bearbeitet werden.

