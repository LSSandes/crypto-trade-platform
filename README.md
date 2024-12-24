# Demo Trading

Advanced cryptocurrencies demo trading platform.
## Features✨

### Market:
- real-time price
- search any cryptocurrency!

### Trade:
- spot trading
- limit-order trading
- recent trades(Live)
- all trade histories
- all open orders
- cancel open orders

### Portfolio:
- account available margin
- account total margin
- PNL chart
- asset allocation chart

### Trade history
- all trade histories

### Open orders:
- all open orders
- cancel orders

### Profile:
- gravatar profile photo
- edit name and last name
- change password
- view email and username

## Tech

All used frameworks, technologies and libraries:

- [Django] - We use django for our backend
- [Redis] - Datebase memory caching and message broker
- [PostgreSql] - Sql datebase
- [JavaScript] - Our frontEnd made with pure js
- [jQuery] - FrontEnd
- [Twitter Bootstrap] - Great UI boilerplate for modern and responsive web apps
- [Heroku] - Deployment
- [Sentry] - Error tracking for both Django/JS
- [Google analytics] - For users analysis
- [Celery] - task schedule
- [Docker] - container
- [Django channels] - socket programming

If you want to pass ci/cd and auto deploy after each commit, you should add below secrets to your github repo secret lists.

| KEY | VALUE |
| ------ | ------ |
| CRYPTO_COMPARE_API | [Get it from here](https://min-api.cryptocompare.com/) |
| EMAIL_HOST_USER | Email username|
| EMAIL_HOST_PASSWORD | Email password |
| SOCIAL_AUTH_GOOGLE_OAUTH2_KEY | [Get it from here](https://developers.google.com/identity/protocols/oauth2) |
| SOCIAL_AUTH_GOOGLE_OAUTH2_SECRET | Secret from above |
| HCAPTCHA_SITEKEY | [Login and create new site](https://dashboard.hcaptcha.com/overview) |
| HCAPTCHA_SECRET | Copy secret from above url |
| SENTRY_DSN | [Follow this instruction](https://docs.sentry.io/platforms/python/guides/django/) |
| HEROKU_API_KEY | Your API key |
| HEROKU_APP_NAME | Your app name to be deployed here |
| HEROKU_EMAIL | Your email address related to your heroku account |

## Celery
```
$ cd web
$ python3 -m celery -A config worker -l info -c 4
```




