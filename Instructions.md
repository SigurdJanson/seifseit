# Hugo

Always use the **extended** version to allows SCSS.



# Structure

* Services?
* About
* Contact
* ...????

# Pages

## Markdown

Use the `param` short code to access variables in markdown files.


## About

The layout is "about.html".

### Arguments

|   |   |
|---|---|
| about |   |
| insight |   |
| funfacts | list |
| features | list |
| testimonials | disabled |
| mission_vision |   |
| cta | true/false |


**Fun facts**. A list of numbers, when these scroll into the viewport they start counting from zero to the designated value. As `count` argument the layout supports numeric values and short codes.


# Theme

Several templates, ... from the theme have been overwritten by templates with the same name in the project folder.

Ionicons version of the theme was v2. I have updated this to [v5.5.2](https://github.com/saulodias/ionicons-font/tree/master).



# Writing Short Codes, Templates, etc.

## Structured Comments

```
{{- /*
  Describe what the short code does

  @param {type} [argumentname=defaultvalue] If true, display a copy to clipboard button.
  @param {string} [config] The section of site.Data.docs.config to render.
  @param {bool} [fm=false] If true, render the code as front matter.

  @returns {...}

  @usage {{< getcontent path="PATH/TO/FILE" >}}
*/}}
```


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



# Hugo Language

Hugo has no built-in function To identify the type of a variable. [Workarounds on Git](https://github.com/kaushalmodi/hugo-debugprint/blob/master/layouts/partials/debugprint.html).


## Shortcodes

The advantage is that shortcodes can be called from within content files (*.md). 

Calls are in the form: `{{< myshortcode param1="value1" param2="value2" >}}` or `{{% myshortcode param1="value1" param2="value2" %}}`. Shortcode arguments can also be anonymous (i.e. no named): `{{< myshortcode "value1" "value2" >}}`.

Limitations:
* We cannot use variables as arguments. Shortcode arguments must be string, int, float, or bool. We cannot pass in code (including shortcodes) that require evaluation.

Further reading:
* [Create your own shortcodes](https://gohugo.io/templates/shortcode-templates/)
* [Shortcode methods](https://gohugo.io/methods/shortcode/)
* [Variables in the context of a shortcode](https://gohugo.io/variables/shortcode/)
