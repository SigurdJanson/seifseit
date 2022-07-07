
# Site


# .htaccess

There are [.htaccess generators](https://websitesetup.org/tools/htaccess-generator/) to make the job easier. Esp. the password protection for files and folders. 

This file needs to be located in the top directory of a site.

It must contain `AddDefaultCharset UTF-8`. If not, the server will not deliver files as utf-8 which breaks umlauts and other characters.

## Sample

```
# Prevent viewing of .htaccess file ##!important
<Files .htaccess>
order allow,deny
deny from all
</Files>

# Prevent directory listings
Options All -Indexes

########## Begin - Spam bot protection
#
RewriteCond %{HTTP_USER_AGENT} ^.*Whacker.*$ [OR] 
RewriteCond %{HTTP_USER_AGENT} ^EmailCollector [OR]
RewriteCond %{HTTP_USER_AGENT} ^EmailSiphon [OR] 
RewriteCond %{HTTP_USER_AGENT} ^EmailWolf [OR] 
RewriteCond %{HTTP_USER_AGENT} ^.*FileHound.*$ [OR]
RewriteCond %{HTTP_USER_AGENT} ^.*TurnitinBot.*$ [OR]
RewriteCond %{HTTP_USER_AGENT} ^.*JoBo.*$ [OR]
RewriteCond %{HTTP_USER_AGENT} ^.*adressendeutschland.*$
# Send all blocked request to homepage with 403 Forbidden error!
RewriteRule ^.* - [F]
#
########### End - Spam bot protection
```

## Hotlink Prevention
When another site creates hotlinks to your images, they’re not only making use of your images, but your bandwidth as well.

```
RewriteEngine on
RewriteCond %{HTTP_REFERER} !^$
RewriteCond %{HTTP_REFERER} !^http://(www\.)seifseit.de/.*$ [NC]
RewriteRule \.(gif|jpg|webp|png)$ - [F]
```



## Password protect file (requires .htpasswd file)

See also https://gooseyman.com/post/2020-05-26_password_protect_hugo_site/

The .htpasswd stores the user name and the password (encrypted).


