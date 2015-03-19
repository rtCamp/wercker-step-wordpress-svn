# wordpress-svn

Wercker deploy step for wordpress.org plugin svn repo

## Usage

```yml
deploy:
  steps:
    - rtcamp/wordpress-svn:
        pluginslug: wordpress.orh plugin plug
        mainfile: main plugin filename for your plugin
        svnuser: wordpress.org username
        svnpass: $WPPASS                     #wordpress.org password
        gituser: github username
        gitpass: $GITHUBPASS                  #github.com password

```

For safety, do not write `` or `$SVNPASS` inside `wercker.yml` file.
