# Netflify: 
 - add file named `_redirects` 
```t
/*    /index.html   200
```

# Cpanel: 
- add file named `.htaccess`
```t
Options -MultiViews
    RewriteEngine On
    RewriteCond %{REQUEST_FILENAME} !-f
    RewriteRule ^ index.html [QSA,L]
```
