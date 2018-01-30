Kris#Pour installer projet en local : 


installer curl puis composer : 

sudo apt-get install curl\ncurl -sS https://getcomposer.org/installer 
sudo php -- --install-dir=/usr/local/bin --filename=composer\ncomposer

Créer un projet themosis
composer create-project themosis/themosis BTDance

Faire un pull et merge tout dans le dossier BTDance créé. 
Aller chercher la bdd dans bdd/ et l'importer dans sa bdd locale. 


dans BTDance/.env.local renseigner les champs : 
DB_NAME = "votre_database"
DB_USER = "votre_username"
DB_PASSWORD = "votre_password"
DB_HOST = "localhost"
WP_HOME = "votre_url"
WP_SITEURL = "votre_url/cms"

dans config/envrionment.php : renseigner les champs: 

   'local' => 'votre_hostname',
   'production' => 'votre_url'


composer install










[![Build Status]
