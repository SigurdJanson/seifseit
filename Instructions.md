
# Hugo

Always use the **extended** version to allows SCSS.



# Site


# .htaccess

There are [.htaccess generators](https://websitesetup.org/tools/htaccess-generator/) to make the job easier. Esp. the password protection for files and folders. 

This file needs to be located in the top directory of a site.

It must contain `AddDefaultCharset UTF-8`. If not, the server will not deliver files as utf-8 which breaks umlauts and other characters.

## The Solution

The solution for humans.txt was taken from a [discourse discussion](https://discourse.gohugo.io/t/htaccess-humans-txt-with-template-logic/27624).

We need an output format for .htaccess and (since the media type "text/htaccess" is no standard type) a user-defined media type:

``` toml
[outputFormats.htaccess]
    baseName = ""
    isPlainText = true
    mediaType = "text/htaccess" # see media types

[mediaTypes]
  [mediaTypes."text/htaccess"]
    suffixes = ["htaccess"]
```

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

The '.htpasswd' stores the user name and the password (encrypted).






# humans.txt

The solution for humans.txt was taken from a [discourse discussion](https://discourse.gohugo.io/t/htaccess-humans-txt-with-template-logic/27624).

The template file is "index.humanstxt.txt". It uses a partial to create the authors. In order for this to work, hugo also needs an output format:

``` toml
[outputFormats.humanstxt]
    baseName = "humans"
    isPlainText = true
    mediaType = "text/plain"
```



# Publications

Publications are listed in JabRef and exported to json. Use the JabRef export feature and save the json to "data/pubs/papers.json".

The format is defined in the hugo folder under "jabref_export\json.layout".
