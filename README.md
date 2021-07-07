$ heroku config:set HEROKU_API_KEY=`heroku auth:token`

$ heroku buildpacks:add heroku-community/cli

$ git push heroku master
...

remote: -----> heroku-cli app detected
remote: === Fetching and vendoring Heroku CLI into slug
remote: === Installing profile.d script
remote: === Heroku CLI installation done
...

$ heroku run 'heroku auth:token'
Running `heroku auth:token` attached to terminal... up, run.3706
abcdef0123456789abcdef0123456789abcdef01

$ heroku run 'heroku pgbackups:capture SILVER -a myapp'
Running `heroku pgbackups:capture SILVER -a myapp` attached to terminal... up, run.9532

HEROKU_POSTGRESQL_SILVER_URL  ----backup--->  b003

Capturing... done
Storing... done
