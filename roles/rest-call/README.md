# Task 3 - Postleitzahl-Auflöser
## Beschreibung
Die Rolle ruft einen Webservice mit der übergebenen Postleitzahl auf.

Aus der Rückgabe des Webservices wird der Ortsname gefiltert und ausgegeben.
Wird zur übergebenen Postleitzahl kein entsprechender Eintrag gefunden, wird
eine Fehlermeldung ausgegeben.

## Parameter
Name | Value
-----|------
zip_code | String mit 5 Zahlen <br/> e.g. zip_code=01099 <br/> default: `04275`