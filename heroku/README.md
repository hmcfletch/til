# Heroku

TIL's about Heroku and its associated tech

### Scratch

* Run detached command: `heroku run:detached rake db:migrate`
* Restart a particular type of dyno `heroku ps:restart worker`
* Open psql `heroku pg:psql -a <APP>`
* `heroku pg:backups capture`
* `curl -o latest.dump \`heroku pg:backups public-url\``
