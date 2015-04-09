# wordpress-svn

Wercker deploy step for wordpress.org plugin svn repo

## Usage

```yml
deploy:
  steps:
    - rahul286/wordpress-svn:
        pluginslug:   hello-world                    #wordpress.org plugin slug
        mainfile:     example.php                    #main plugin filename
        svnuser:      wpusername                     #wordpress.org username
        svnpass:      $SVNPASS                       #wordpress.org password
        gituser:      githubusername                 #github.com username
        gitpass:      $GITPASS                       #github.com password
```

For safety, do not write `GITPASS` or `SVNPASS` inside `wercker.yml` file. Instead use [pipeline or deploy variables](http://old-devcenter.wercker.com/articles/steps/variables.html)
