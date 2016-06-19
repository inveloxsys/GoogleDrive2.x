# GoogleDrive2.x
// ===============================================
/**
 * # Google Drive volume driver need "google-api-php-client"  latest version package"
 * * google-api-php-client: https://github.com/google/google-api-php-client
 * * copy directory "google-api-php-client" and paste in elFinder php directory
 * * Google Drive developer console: https://console.developers.google.com
 * * Create login in google developer console and create app and get clientid, clientsecret, redirecturi
 * * create new project ->Enable and manage APIs ->Drive API ->Enable ->Goto Credentials
 * * Create Credentials ->oAuth Client ->web Applicaton
 * */ 
 // Required for Google Drive Netmount
 // Installation by composer
 // `composer require googledrive/googledrive2.x`
 // Enable network mount
 // with autoload
 elFinder::$netDrivers['googledrive'] = 'GoogleDrive';
 // without autoload
 include_once dirname(__FILE__).DIRECTORY_SEPARATOR.'elFinderVolumeGoogleDrive.class.php';

 // GoogleDrive Netmount driver need next two settings. You can get at https://console.developers.google.com
 // AND reuire regist redirect url to "YOUR_CONNECTOR_URL?cmd=netmount&protocol=googledrive&host=1" 
 define('ELFINDER_GOOGLEDRIVE_CLIENTID', 		'');
 define('ELFINDER_GOOGLEDRIVE_CLIENTSECRET',	'');
// ===============================================
