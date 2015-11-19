# Camunda BPM Rest API

Camunda Process Engine and REST API running in servlet container.

## Installation

1. Create PostgreSQL `bpmsample` user and database with `bpmsample` password
2. Install Apache Tomcat
2. Build the project
    $ mvn install
3. Copy the resulting WAR file to Apache Tomcat's `webapps` directory

## Deploying on Heroku

    $ heroku create
    $ heroku git:remote -a <application_name>
    $ heroku ps:scale web=1
    $ heroku addons:create heroku-postgresql:hobby-dev
    $ git push heroku master
      OR
    $ mvn heroku:deploy-war

## License

[Apache 2.0 License](http://www.apache.org/licenses/LICENSE-2.0)
