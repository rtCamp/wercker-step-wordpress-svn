# wordpress-svn

Wercker deploy step for wordpress.org plugin svn repo

## Usage

```yml
deploy:
  steps:
    - rahul286/wordpress-svn:
        pluginslug:   wordpress.org plugin plug
        mainfile:     main plugin filename for your plugin
        svnuser:      wordpress.org username
        svnpass:      $SVNPASS                     #wordpress.org password
        gituser:      github username
        gitpass:      $GITPASS                  #github.com password
```

For safety, do not write `GITPASS` or `SVNPASS` inside `wercker.yml` file. Instead use [pipeline or deploy variables](http://old-devcenter.wercker.com/articles/steps/variables.html)
