# Task 4 - NGiNX Configuration
## Beschreibung
Die Rolle erstellt eine NGiNX-Konfiguration mit definierbaren `location`-Entries an.

Für jeden `location`-Entry wird ein Verzeichnis mit entsprechendem Name als www-home
Verzeichnis angelegt.

Die `location`-Entries der NGiNX-Config lassen sich im Template `templates/nginx-location.conf.j2` anpassen.

## Templates
Template | Beschreibung
-----|------
index.html.js2 | Template für die index.html
nginx-base.conf.j2 | Template NGiNX-Basis-Konfiguration <br/> am Marker ### ANSIBLE GENERATED ### werden die `location`-Entries eingefügt
nginx-location.conf.j2 | Template für die zu erzeugenden `location`-Entries

## Parameter
Name | Value
-----|------
locations | Liste der anzulegenden NGiNX `location`-Entries <br/> default: `- folder1`
path_nginx_config | Pfad, in dem die NGiNX-Config angelegt wird <br/> default: `/etc/nginx/sites-available/`
path_www_home | Pfad, in dem die Ordner für www-home angelegt werden <br/> default: `/var/www/nginx-demo/`
filename_nginx_config | Dateiname der NGiNX-Config <br/> default: `default.conf`
