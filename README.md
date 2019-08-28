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


## Does this interest you?

<a href="https://rtcamp.com/"><img src="https://rtcamp.com/wp-content/uploads/2019/04/github-banner@2x.png" alt="Join us at rtCamp, we specialize in providing high performance enterprise WordPress solutions"></a>
