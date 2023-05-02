# NGINX Notes
## NGINX.conf is a just a demo that includes most of what I learned
<br>

- NGINX start
```
nginx
```
- NGINX reload
``` 
nginx -s reload
```
<br>

NGINX conf file has
- directive (like a key value)
- context: contains directives

<br>

### We use ```#``` for comments

<br>

### Dealing with http the conf file will need two contexts
- ```http{}``` with a ```server{}``` context inside
- ```events{}```

### Check the config file then follow up with notes again

<br>

if the subdomain doesn't have an index.html we can use ```try_files``` to address other files or put an error message

```
try_files /sub_domain/another_index.html /try_this_secondly.html /so_on.html =<error number>;
```

