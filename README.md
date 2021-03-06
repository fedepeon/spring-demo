
# Spring Demo
it is a basic web app, written using **Spring Boot**.

## Build
Run `mvn package` to build the project, this will create a single file
in `target/spring-demo-VERSION.jar`. Then you can start the server, using:
```bash
java -jar target/spring-demo-VERSION.jar
```

## Development
You can get *hot reload* in both the server and the frontend. In order to
do this, run the main class of the app with your IDE (or using `mvn spring-boot:run`)
and then run `yarn start` in the `src/main/webapp` folder. It should run in <http://localhost:8080/>.

## Running the Tests
If you want to check that it just work, run `mvn verify`.
Also, to run only the unit test, use `mvn test`. And to run only
the integration tests, use  `mvn failsafe:integration-test`.

## Documentation
The documentation of the **REST API** is built automatically on `mvn package`. You can see it
by running the server and going to <http://localhost:8080/docs>.

Also, you can see it after a `mvn prepare-package`, that will run the tests and generate the documentation
into `target/generated-docs/index.html`.

## Built With
* [Java](https://www.java.com/download/) - Programming Language
* [Maven](https://maven.apache.org/download.cgi) - Dependency Management and Build Tool
* [Spring Boot](https://projects.spring.io/spring-boot/) - Java Web Framework
* [H2](https://www.h2database.com/html/main.html) - Embedded Database (development)
* [PostgreSQL](https://www.postgresql.org/) - Relational Database
* [Webpack](https://webpack.js.org/) - JavaScriptModule Bundler
* [Yarn](https://yarnpkg.com/docs/install) - JavaScript Package Manager
* [Vue](https://vuejs.org) - JavaScript UI Framework

## Author
* **Gustavo Paulo** - [gpaulo00](https://github.com/gpaulo00)
