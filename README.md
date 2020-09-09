# Codeception visual base

## This is a base project for codeception visual testing

It should provide webdriver ready to make tests on existing website.

To run some test:
1. replace webdriver `url` in acceptance.suite.yml
2. create an external network: `docker network create proxy`
3. start docker compose: `docker-compose up -d`
4. install dependencies: `docker exec -it codeception_visual composer install`
5. write some codeception acceptance tests
6. run tests `docker exec -it codeception_visual php vendor/bin/codecept run`