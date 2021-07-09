# Heroku Buildpack for SQ1

Installs SQ1 and WordPress utilities and dependencies:

* WPCLI
* Export PHP bin for CLI use

## Configuration 

Creates a `Procfile` if doesn't exists one at the root folder and copy some default configurations for `nginx`, `php-fpm` and `php.ini`. 

Features:
* `nginx` - sets root directory to the wordpress under the subfolder `wp/`. 
* `php-fpm` - set `pm` to static and limits to `10` processes. 
* `php.ini` - set `upload_max_filesize` to 50M.
