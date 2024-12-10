# Java

## Install JDK Amazon Corretto 17
[https://docs.aws.amazon.com/corretto/latest/corretto-17-ug/what-is-corretto-17.html](https://docs.aws.amazon.com/corretto/latest/corretto-17-ug/what-is-corretto-17.html)

- Add `JAVA_HOME` environment variable
- Add `JAVA_HOME/bin` to `PATH` environment variable

### Java version
```sh
java -version
```

## Maven
Maven is a build and project management tool primarily used for Java projects but also supports other JVM-based languages. It simplifies tasks such as dependency management, compilation, testing, and packaging of applications.

### Install Maven
[https://maven.apache.org/download.cgi](https://maven.apache.org/download.cgi)

- Add `M2_HOME` environment variable to point to your maven folder path
- Add `M2_HOME/bin` to `PATH` environment variable

### Useful command
Maven Version
```sh
mvn -version
```

Package (builds project, runs test, creates artifacts)
```sh
mvn package
```
Install dependencies (builds project, runs test, installs artifacts(jars,poms, wars) to local repository)
```sh
mvn install
```

Clean (removes working directories `target`)
```sh
mvn clean
```

### Set up maven with JFrog
1. Go to [https://p6m.jfrog.io](https://p6m.jfrog.io)
2. Login
3. Profile → Set me Up → Maven → Generate Token and Create Instructions → Generate Settings → Download Snipped
4. Move `settings.xml` to your `~/.m2`  folder