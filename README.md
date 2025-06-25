* Welche Schritte waren notwendig, um Jenkins lokal mit Docker zum Laufen zu bringen?

A: 1. Jenkins Master als Docker-Container starten und ein benanntes Volume für die Daten verwenden
    2. Im Browser localhost:8080 öffnen und die Installation abschließen 
    3. In Jenkins einen neuen Pipeline-Job erstellen.

* Was ist der Zweck der Datei Jenkinsfile, und wo muss sie im Verhältnis zu deinem Anwendungscode liegen?

A: DIe Jenkinsfile definiert die Pipeline für Jenkins. Sie beschreibt, wie der Build-Prozess ablaufen soll. Die Datei muss im Wurzelverzeichnis meines Anwendungscodes liegen.

* Beschreibe die zwei Hauptstages, die du in deiner Pipeline definiert hast, und was der Hauptzweck der Steps in jeder Stage ist. 

A: install dependencies - alle nötigen Pakete mit npm ci werden installiert.
    Build - mit npm run build wird die Anwendung gebaut 

* Wie hast du in Jenkins konfiguriert, von welchem Git-Repository und welchem Branch der Code für die Pipeline geholt werden soll? 

A: Ich habe die URL meines GitHub-Repos hinzugefügt und festgelegt, dass der main-Branch verwendet werden soll.

* Was ist der Unterschied zwischen dem checkout scm Step in deiner Pipeline und dem git clone Befehl, den du manuell im Terminal ausführen würdest?

A: checkout scm lädt in Jenkins automatisch den Code aus dem Git-Repo. git clone ist ein Befehl, den man selbst im Terminal ausführen muss