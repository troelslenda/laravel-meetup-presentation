# Developing with Docker

This is the demo script for the presentation Developing with Docker i gave at the Laravel meetup in February 2018. Slides are available here. https://docs.google.com/presentation/d/1075n7U-KskxhNid80KBB4jnzHZ4Px-ug2MkqT3mgzk8/edit?usp=sharing

## Demo setup

Make sure to install Docker CE for Mac. Now docker and docker-compose binaries should be avaliable in your terminal.

To get up and running execute `docker-compose up` in this directory.

in a new terminal window execute ` docker-compose exec app composer create-project laravel/laravel .` to download Laravel

When downloaded edit `./web/.env` and replace `DB_HOST=127.0.0.1` with `DB_HOST=database`

Make artisan executeable within container by `chmod a+x web/artisan`. Then you can execute it by running `docker-compose exec app ./artisan`

You can hit localhost:8080 in your browser.