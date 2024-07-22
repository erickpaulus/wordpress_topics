# Wordpress
Address an login issue in Stagging mode.

```
The issue is present due to the custom values in your `wp-config.php` file enforcing the live site domain to be used:
you can remove or give comment sign on these code line :

#$web_site     = 'www.yourdomainname.com';
#$schema       = isSecure() ? 'https://' : 'http://';
#$web_site_url = $schema . $web_site;

#define('WP_HOME',    $web_site_url);
#define('WP_SITEURL', $web_site_url);
```
