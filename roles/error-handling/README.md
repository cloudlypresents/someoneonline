# Task 2 - Error Handling
## Beschreibung
Die Rolle führt ein Directory-Listing mit dem Befehl `ls` aus.

Um zu demonstrieren, dass die Rolle im Fehlerfall durchläuft, wird
der Pfad `/nothing/here` als default verwendet. 

Die Fehlermeldung wird ins Log-File unter dem angegeben Pfad geschrieben. 

Wird keine Fehlermeldung erzeugt, wird die Rückgabe des Befehls als
Debug-Message ausgegeben.

## Parameter
Name | Value
-----|------
check_path | String <br/> default: `/nothing/here`
error_folder | String für Dateipfad des Error-Log <br/> default: `error-debugging`