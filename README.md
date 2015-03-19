# wordpress-svn

Wercker deploy step for wordpress.org plugin svn repo

## Usage

```
deploy:
  steps:
    - rtcamp/wordpress-svn:
        svnuser: wordpress.org username
        svnpass: $SVNPASS
        pluginslug: wordpress.orh plugin plug
        mainfile: main plugin filename for your plugin
        
```

For safety, do not write `svnpass` or `$SVNPASS` inside `wercker.yml` file. 
