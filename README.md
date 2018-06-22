MODULE
------
Basic page node's to json using a site wide API key

CREDITS
-------------
Developed by : Sunny Sharma 
<infoofsunnysharma@gmail.com>

https://www.drupal.org/u/sunnydrupal

JSON Encode URL
-----------------
URL : http(s)://sitename/node_json/SITEAPIKEY/<NODE_ID>
test url : http://sitename/node_json/SITEAPIKEY/<NODE_ID>

REQUIREMENTS
-------------
1) Alter Site information page in admin with field name 'Site API Key' under 'Site Detail' Section.
2) Make 'Site API key' is compulsory field.
3) Button text 'Save configuration' should be changed to 'Update configuration' at the time of updating key.
4) Create page using custom code which uses Site API key as parameter in URL.
5) If API key is present in URL, It would return content of content type 'Basic page' in json format.
6) If API Key is not present in URL, it would return Access denied.
7) If content type is not 'Basic page', it would return Access denied.

References
-------------
Form API : 
https://www.drupal.org/docs/8/api/form-api/introduction-to-form-api

Configuration API : 
https://www.drupal.org/docs/8/api/configuration-api/configuration-api-overview

EntityTypeManager :
https://api.drupal.org/api/drupal/core%21lib%21Drupal.php/function/Drupal%3A%3AentityTypeManager/8.2.x

JsonResponse : 
https://api.drupal.org/api/drupal/vendor%21symfony%21http-foundation%21JsonResponse.php/class/JsonResponse/8.2.x
