# Blogger Advanced

This is a sample project for use with the tutorials at http://tutorials.jumpstartlab.com

Please do _not_ take it as a set of best practices. In fact, there are many intentional inefficiencies or points of ugliness setup for "fixing" through [tutorial exercises](http://tutorials.jumpstartlab.com/projects/ruby.html).


## Getting Started

```bash
git clone git://github.com/JumpstartLab/blogger_advanced.git
cd blogger_advanced
bundle
rake db:migrate
rails server
```

OR

Install [Docker](https://www.docker.com/products/docker-desktop).

Then:

```bash
git clone git://github.com/JumpstartLab/blogger_advanced.git
cd blogger_advanced
docker-compose build
docker-compose run web rake db:migrate db:create db:seed
docker-compose up
```

At this point your server should be running allowing you to visit `localhost:3000`

If you would like to use rails commands, preface them with `docker-compose run web`. For example:

```bash
docker-compose run web rails c
```

## Branches

There are some branches to show some functionality.

* bootstrap: it's the updated Blogger. It will probably be merged into master soon.
* api: shows a single responsibility API controller for the articles.
* secure_api_with_basic_auth: implements basic authentication for the API articles controller.
* secure_api_with_http_token: implements http token authentication for the API articles controller.

## Contribute

If you find something that is outdated or doesn't work, feel free to submit a pull request. All contributions are greatly appreciated.
