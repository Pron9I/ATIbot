worker: npm start
heroku login vladpron2016@gmail.com WOwnib846_
heroku stack:set cedar-14
heroku buildpacks:add --index 1 https://github.com/heroku/heroku-buildpack-apt
heroku buildpacks:add --index 2 https://github.com/captain401/heroku-buildpack-xvfb.git
heroku buildpacks:add --index 3 https://github.com/causztic/heroku-electron-buildpack.git
heroku buildpacks:add --index 4 https://github.com/heroku/heroku-buildpack-nodejs.git
heroku create --region eu atibot1
heroku addons:create heroku-redis:hobby-dev -a atibot1
git push heroku master
heroku ps:scale web=0
heroku ps:scale bot=1 # запускаем бота
heroku logs --tail