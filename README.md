# W24-4PM-4-Team01

Lab instructions: <https://ucsb-cs156.github.io/w24/lab/team01.html>


|   Name          | GitHub Id     |  Service                    | Controller                |
|-----------------|---------------|-----------------------------|---------------------------|
|Rohan Morangoly  |rmarangoly     | `LocationQueryService`      | `LocationController`      |
|Alexander Nguyen |anguyen412     | `PublicHolidayQueryService` | `PublicHolidayController` |
|Hongye Liang     |hongye-liang   | `TidesQueryService`         | `TidesController`         |
|Justin Zhang     |JustinZhang809 | `UniversityQueryService`    | `UniversityController`    |
|Kole Kikuta      |ktkikuta       | `ZipCodeQueryService`       | `ZipCodeController`       |
|Hao Yi           |hyi96          | `JokeQueryService`          | `JokeQueryController`     |


Repo: (https://github.com/ucsb-cs156-w24/team01-w24-4pm-4.git)

On Dokku: http://team01.dokku-04.cs.ucsb.edu/swagger-ui/index.html

## About this repo

This is a minimal backend only webapp built with Spring Boot.

The app provides some sample code for an API, and a Swagger user interface
to test that API.  The API is essentially a proxy for another API.

This code is the basis for a programming exercise where each student on a
team of up to 5 students can build a proxy similar to the one in the example code.

## What can you do with this code?

| Command | What it does   |
|----------|---------------------------------------|
| `mvn compile` | Should result in a clean compile |
| `mvn test` | Runs JUnit tests on the code base |
| `mvn test jacoco:report` | Runs JUnit tests, and if all tests pass, computes code coverage.  The code coverage report (Jacoco) can be found in `target/site/jacoco/index.html` |
| `mvn package` | Builds the jar file `target/team01-spring-boot-1.0.0.jar` |
| `mvn spring-boot:run` | Runs the code to startup a web server.  Access it via `http://localhost:8080` on the *same machine* where the server is running.  Use CTRL/C to stop it. |
| `java -jar target/team01-spring-backend-1.0.0.jar` | If done after `mvn package`, this is another way to start up the web server.|
| `mvn test pitest:mutationCoverage` | Run [pitest mutation coverage](https://pitest.org).  View `target/pit-reports/index.html` for results (may take a few minutes)|

# Deploying on Dokku

For advice on deploying on Dokku, see: [/docs/dokku.md](/docs/dokku.md)

