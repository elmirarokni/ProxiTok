[![Deploy](https://www.herokucdn.com/deploy/button.svg)](https://heroku.com/deploy)
# ProxiTok
Use Tiktok with an alternative frontend, inspired by Nitter.

## Features
* Privacy: All requests made to TikTok are server-side, so you will never connect to their servers
* See user's feed
* See trending and discovery tab
* See tags
* See video by id
* Themes
* RSS Feed for user, trending and tag (just add /rss to the url)

## Self-hosting
Please check [this](https://github.com/pablouser1/ProxiTok/wiki/Self-hosting) wiki article for info on how to self-host your own instance

## Public instances
[This](https://github.com/pablouser1/ProxiTok/wiki/Public-instances) wiki article contains a list with all the known public instances.

## Extensions
If you want to automatically redirect Tiktok links to ProxiTok you can use:
* [Libredirect](https://github.com/libredirect/libredirect)
* [Redirector](https://github.com/einaregilsson/Redirector)

You can use the following config if you want to use Redirector (you can change https://proxitok.herokuapp.com with whatever instance you want to use):
```
Description: TikTok to ProxiTok
Example URL: https://www.tiktok.com/@tiktok
Include pattern: (.*//.*)(tiktok.com)(.*)
Redirect to: https://proxitok.herokuapp.com$3
Example result: https://proxitok.herokuapp.com/@tiktok
Pattern type: Regular Expression
Apply to: Main window (address bar)
```

## TODO / Known issues
* Make video on /video fit screen and don't overflow
* Fix embed styling
* Fix crash when invalid vm.tiktok.com/CODE or www.tiktok.com/t/CODE is provided
* Add custom amount of videos per page

## Credits
[@TheFrenchGhosty](https://github.com/TheFrenchGhosty): Initial Dockerfile and fixes to a usable state. You can check his Docker image [here](https://github.com/PussTheCat-org/docker-proxitok-quay) on Github or [here](https://quay.io/repository/pussthecatorg/proxitok) on Quay
### External libraries
* [TikScraperPHP](https://github.com/pablouser1/TikScraperPHP)
* [Latte](https://github.com/nette/latte)
* [bramus/router](https://github.com/bramus/router)
* [PHP dotenv](https://github.com/vlucas/phpdotenv)
* [Bulma](https://github.com/jgthms/bulma) and [Bulmaswatch](https://github.com/jenil/bulmaswatch)
