worker: npm start
heroku login vladpron2016@gmail.com WOwnib846_
heroku create --region eu atibot1
heroku addons:create heroku-redis:hobby-dev -a atibot1
git push heroku master
heroku ps:scale web=1
heroku ps:scale bot=1 # запускаем бота
heroku logs --tail