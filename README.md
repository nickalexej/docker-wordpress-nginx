# DEV Vorlage für Wordpress

Vorlage für Docker mit NGINX Proxy + REDIS Cache.

## Installation
Hier MUSS in der ````config/default.conf```` Datei die Server URL unter ````server_name```` angepasst werden.

Nach der Installation von Wordpress passt man nun für REDIS die ````wp_config.php```` an. In der DEFINE Sektion wird die Zeile
`````
define( 'WP_REDIS_HOST',    'wordpress-cache');
`````
hinzugefügt. Nun installiert man noch das Plugin [Redis Object Cache](https://de.wordpress.org/plugins/redis-cache/) und aktiviert dies.
