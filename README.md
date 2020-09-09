# Codeception visual base

## This is a base project for codeception visual testing

It should provide webdriver ready to make tests on existing website.

To run some test:

1. write some codeception acceptance tests
2. replace webdriver `url` in acceptance.suite.yml
2. start docker compose: `docker-compose up -d`
3. run tests `docker exec -it codeception_visual php vendor/bin/codecept run`